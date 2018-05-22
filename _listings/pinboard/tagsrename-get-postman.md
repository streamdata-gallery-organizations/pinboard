{
  "info": {
    "name": "Pinboard Rename Tags",
    "_postman_id": "876b0765-7700-4915-a5d7-e65b7911b95c",
    "description": "Rename an tag, or fold it in to an existing tag.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Posts",
      "item": [
        {
          "id": "cdae9cf2-9ed9-488b-840b-01b378359625",
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
              "id": "fc8a7543-9580-48ea-ac3a-c0ced2eee94c"
            }
          ]
        },
        {
          "id": "c6a4d431-c420-4c59-bb4f-c119e4bfb520",
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
              "id": "e79f50e0-ca33-4e47-9d16-29ca764c10a0"
            }
          ]
        },
        {
          "id": "34a5f1a4-ba50-4c7b-9338-9587ec1c94db",
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
              "id": "025b5e0a-92ea-4087-9a76-027be91fb191"
            }
          ]
        },
        {
          "id": "d0ffa697-2841-45bc-b456-926985f50070",
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
              "id": "b4f94f64-a57d-42b6-a335-3ae0ee37dcd9"
            }
          ]
        },
        {
          "id": "cf720c0d-d114-48fd-87d0-009edb0bb663",
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
              "id": "2f18d9bb-3c38-4a07-bd84-847281abf8ac"
            }
          ]
        },
        {
          "id": "1c5ecfa7-5423-4ed7-aadc-f82df0bcaad2",
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
              "id": "b2738d44-4011-4b7c-84fd-d0c47ea003a6"
            }
          ]
        },
        {
          "id": "e18d9c6b-5c27-4d22-accb-1c0911a9a180",
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
              "id": "d5f91f54-1326-442c-ad7e-6868866a29ab"
            }
          ]
        },
        {
          "id": "553146ae-cc34-4d1a-b8de-6e7c5535fff5",
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
              "id": "857d9de8-2c2b-4223-9179-8e42fe1ebd14"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "c4f56288-1c2e-420b-bc63-40443350af97",
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
              "id": "88c487ea-4677-41f3-9cd1-9bf43cc43df5"
            }
          ]
        },
        {
          "id": "0ce6854a-6f81-46b7-871f-68086add435f",
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
              "id": "2073cbe9-61b5-4598-82f4-3380d945331e"
            }
          ]
        },
        {
          "id": "848e2515-3454-49c9-9227-e49b7d775558",
          "name": "tags.rename.get",
          "request": {
            "url": "http://api.pinboard.in/v1/tags/rename",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Rename an tag, or fold it in to an existing tag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e971bf55-f9a4-463e-85cb-bfae71652798"
            }
          ]
        }
      ]
    }
  ]
}