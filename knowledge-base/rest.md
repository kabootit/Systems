# Rest

## 7 Rules for REST API URI Design

### Blog: http://blog.restcase.com/7-rules-for-rest-api-uri-design/

1. A trailing forward slash (/) should not be included in URIs
2. Forward slash separator (/) must be used to indicate a hierarchical relationship
3. Hyphens (-) should be used to improve the readability of URIs
4. Underscores (_) should not be used in URIs
5. Lowercase letters should be preferred in URI paths
6. File extensions should not be included in URIs
7. Should the endpoint name be singular or plural?

### HN: https://news.ycombinator.com/item?id=14579248

> REST is easy when you're just doing CRUD. It's once you have actions besides "update" that things start to get a bit more interesting.

I disagree, it's fairly simple, people only find it hard because they're thinking in RPC terms - in commands instead of resources.

An action is simply a new resource you create. You don't send_emails(), you create a new email sending resource, which has its own URL you can check in later (giving you built-in resilience to network cuts and other problems).

Generally, trying to treat the server as a dumb API doesn't work well. If your client is the one who knows that something was confirmed, it should tell the server that, and let it worry about sending whatever emails it wants.

So you'd just PUT your resource with state=confirmed, and let the server take care of any side effects that might trigger.

On the other hand, if it's something like a mass email created by the user, then the client should POST to create a new "mass mailing resource", then it'd PUT all the changes made by the client, and finally PUT its state to "ready to send" so that the server can do so.

## Just use GraphQL Camp

Comment: https://news.ycombinator.com/item?id=14580064

> We've recently started our transition from full rest to graphql. It's actually magical how much easier it is to do everything.
>
> We've used join-monster to handle the sql generation so it's been a breeze to get everything up and running.
>
> Its surprising how fast it is too. We used to use sequelize glasses an orm, but we were getting 4-500ms r times on simple requests. Now for the most part we get sub 100ms responses on complex queries.

## The Deeper Problem

Comment: https://news.ycombinator.com/item?id=14579968

> I think the problem goes deeper then REST & GraphQL, it boils down all the way to SQL and not a lot of people are seeing the problem because it is a "boiling frog" problem. Let me explain. So only a decade ago, all of the work was being done on the server and everything was great (... in a way :), and that's because there you had SQL and you could ask quite complicated questions with it. Now along comes XMLHttpRequest and the iPhone and a lot of the "business logic" starts moving to the frontend slowly. It was a natural thing to do when you need just a little info from the server, basically make "GET /items/1" mean "SELECT * FROM items WHERE id=1", because if you strip all the auth stuff away, that is the essence of that URL. So REST is born. It worked for a while, while the frontend code wasn't doing a lot. But now, we are in a state where everything is being done by the fronted. Now remember all those complicated questions we had to ask of our data, they did not go away, but one thing did, SQL, and all that remained was REST. REST maps to a very limited subset of SQL power, basically all it can do (and still be RESTful) is generate queries like this "SELECT * FROM items WHERE cond1, cond2 ...". Devs were used to working mostly only with queries like this (and ignore joins) because the db was close and there was no (big) penalty for firing 100 queries like these, but now when things moved to the frontend, people started remembering they need to take network latency into account and suddenly "getting everything in one go" ... which is basically a join, became important again. This is what sparked the GraphQL popularity, getting everything in one step, aka ability to express a join everything else is not that important (standard/tooling/types is of course important but it could have been invented for REST also).
>
> Having said all that, GraphQL is still far from the expressivity of SQL and people will still wonder how can they express in GraphQL questions that are easily answered by SQL. Everybody is still thinking in terms of "defining an api" but recently a new way of thinking about this problem started to emerge. Defining a way to translate a HTTP request to a SQL query, i.e. trying to expose the power of SQL in a safe way to the frontend. There is no predefined list of endpoints/types, every requests gets transformed to a SQL query and executed. This is what PostgREST [1] is doing. I know it sounds scary and dangerous but it works :) Try the Starter Kit [2] to get a taste and if GraphQL is your thing, you could explore the same idea using subZero [3]
>
> [1] https://github.com/begriffs/postgrest
> [2] https://github.com/subzerocloud/subzero-starter-kit
> [3] https://subzero.cloud