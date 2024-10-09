Steps:

* `npm run live` this will work as we're on .170

* Change `next` version in package.json from `15.0.0-canary.170` to `15.0.0-canary.171`,
  * `rm -rf node_modules && npm install`
  * `npm run live`
  * Should result in this error:
```
Type error: Route "src/app/api/inngest/route.ts" has an invalid "GET" export:
  Type "ServerResponse<IncomingMessage> & { send: Send<any>; json: Send<any>; ... 5 more ...; revalidate: (urlPath: string, opts?: { ...; } | undefined) => Promise<...>; }" is not a valid type for the function's second argument.
```


