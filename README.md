# cs360-lab8

## Hosting

This server is currently hosted at [http://ec2-52-26-12-151.us-west-2.compute.amazonaws.com:3006/](http://ec2-52-26-12-151.us-west-2.compute.amazonaws.com:3006/)

## Rest Services provided

## `POST /comment`

Format:
```javascript
{
  "Name": string,
  "Comment": string
}
```

Stores the given comment in the mongo database

## `GET /comment`

Response format:
```javascript
[
  {
    __v: number,
    Name: string,
    Comment: string,
    _id: hex_number
  },
  ...
]
```

## Creative Part: `GET /comment?name=`

By add a name parameter to the `GET` request on the `/comment` route, the server will respond with comments only given by the particular name.

