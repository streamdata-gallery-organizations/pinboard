{
  "info": {
    "name": "Pinboard Deletes Tag",
    "_postman_id": "0a1d1425-7b55-4d52-b270-5e0d1ce4349b",
    "description": "Delete an existing tag.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Posts",
      "item": [
        {
          "id": "891d47a0-9942-466e-b8e4-babf89414a4d",
          "name": "posts.update.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/update",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the most recent time a bookmark was added, updated or deleted. Use this before calling posts/all to see if the data has changed since the last fetch."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8722a62-7655-4335-9d38-8acb7c769303"
            }
          ]
        },
        {
          "id": "b5c0619a-7af1-4950-9f6a-0162b813bf36",
          "name": "posts.add.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/add",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Add a new bookmark."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e68627a-6ffc-49ca-b6b5-aa10ea33f54b"
            }
          ]
        },
        {
          "id": "44f9c693-3b1d-4f1d-affa-33f3381cb2dc",
          "name": "posts.delete.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/delete",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a bookmark."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7225d1b0-465b-4ca2-9e14-b6c43be7710b"
            }
          ]
        },
        {
          "id": "73356577-8a72-49f3-aca4-2933f8ef7d59",
          "name": "posts.get.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/get",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns one or more posts on a single day matching the arguments. If no date or url is given, date of most recent bookmark will be used."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7932c4be-e7a1-48e9-9965-085baad19224"
            }
          ]
        },
        {
          "id": "1ee0e9e2-a76e-470f-bbc9-14f4390c02ed",
          "name": "posts.dates.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/dates",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of dates with the number of posts at each date."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3cb3bb3e-2569-4260-b26f-49471f2e85d4"
            }
          ]
        },
        {
          "id": "b6349695-62f6-4ed1-9e57-f5921f3c1a0a",
          "name": "posts.recent.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/recent?count=count&tag=tag",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the user's most recent posts, filtered by tag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8037565a-b5ef-4987-a60d-5e8acd2a4873"
            }
          ]
        },
        {
          "id": "4d5d9857-2417-45c0-9aa0-fe78911a40ac",
          "name": "posts.all.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/all?fromdt=fromdt&meta=meta&results=results&start=start&tag=tag&todt=todt",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all bookmarks in the user's account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03e6d639-625f-4dfa-932f-e16c501646e9"
            }
          ]
        },
        {
          "id": "8c5c6671-97f9-4193-9887-66a1c84e6163",
          "name": "posts.suggest.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/suggest?format=format&url=url",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of popular tags and recommended tags for a given URL. Popular tags are tags used site-wide for the url; recommended tags are drawn from the user's own tags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "145652fc-264e-44be-800b-ca37fa6e389d"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "957665ad-ec28-4863-b882-8c6e737c86dc",
          "name": "tags.get.get",
          "request": {
            "url": "http://api.pinboard.in/v1/tags/get?format=format",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a full list of the user's tags along with the number of times they were used."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fee2858a-5373-4edb-850e-6802ff81f40b"
            }
          ]
        },
        {
          "id": "33d0ab90-6e38-40ad-9a2c-ec2cbc33488c",
          "name": "tags.delete.get",
          "request": {
            "url": "http://api.pinboard.in/v1/tags/delete",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an existing tag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ec7ad3e-eb23-4c46-93a1-628de268bad4"
            }
          ]
        }
      ]
    }
  ]
}