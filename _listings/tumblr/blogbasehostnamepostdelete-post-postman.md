{
  "info": {
    "name": "Tumblr Add Blog Base Hostname Add Delete",
    "_postman_id": "992524c1-eaab-45a3-aaa7-adccaee5f421",
    "description": "Deletes a post.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blog",
      "item": [
        {
          "id": "bdfa9248-d1ae-400f-aaf3-89a8674b97e7",
          "name": "blog.base_hostname.info.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/info"
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This method returns general information about the blog, such as the title, number of posts, and other high-level data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a0e0a3c-813c-4ec4-89aa-170c927320d2"
            }
          ]
        },
        {
          "id": "1f5bb427-5887-4275-a164-6977b30e01ff",
          "name": "blog.base_hostname.avatar.size.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/avatar/:size"
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                },
                {
                  "id": "size",
                  "value": "size",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a blog's avatar in one of 9 different sizes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64d0c146-e063-46aa-9bd3-a9eba595bed5"
            }
          ]
        },
        {
          "id": "2bd86d20-d92d-41bd-864a-a98f736067f5",
          "name": "blog.base_hostname.followers.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/followers"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a blog's followers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32064fee-8fa5-4e11-a1ae-bcab68e7c343"
            }
          ]
        },
        {
          "id": "d0f6a4c4-c9ab-4090-9269-bf39341340b2",
          "name": "blog.base_hostname.posts.type.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/posts/:type"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "notes_info",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "reblog_info",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tag",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                },
                {
                  "id": "type",
                  "value": "type",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves published posts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb65540a-ee67-4222-8df9-ea1e11ed46ea"
            }
          ]
        },
        {
          "id": "f019c568-9b15-45b6-82d9-e1785af58f2c",
          "name": "blog.base_hostname.posts.queue.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/posts/queue"
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves queued posts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75546001-3699-4301-927a-4420e5686cd9"
            }
          ]
        },
        {
          "id": "1bbbe95e-551a-4f36-a9ec-85f681afd425",
          "name": "blog.base_hostname.posts.draft.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/posts/draft"
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves draft posts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "240ca1e1-393d-46d8-988d-d33ba9dd5299"
            }
          ]
        },
        {
          "id": "354dd5b5-3cb8-4e17-a0ae-06ec3064ae1c",
          "name": "blog.base_hostname.posts.submission.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/posts/submission"
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves submission posts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c55655a-d8fe-4f8f-8110-5f63d95f1497"
            }
          ]
        },
        {
          "id": "a36a71a4-5483-4f3c-981e-fbc7433f65b4",
          "name": "blog.base_hostname.post.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/post"
              ],
              "query": [
                {
                  "key": "caption",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "data",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "embed",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "markdown",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tags",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tweet",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new video blog post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9fabc4e-11ea-4d2d-9c3a-0f55334558f7"
            }
          ]
        },
        {
          "id": "134f2f43-3dc6-49c4-9f3f-d0ab0290138b",
          "name": "blog.base_hostname.post.edit.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/post/edit"
              ],
              "query": [
                {
                  "key": "date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "markdown",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tags",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tweet",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Edits a blog post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf083368-4ce1-4967-9ee9-bc73d3aaeb67"
            }
          ]
        },
        {
          "id": "851171ca-abc0-4631-82fc-f5e4106d8a9a",
          "name": "blog.base_hostname.post.reblog.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/post/reblog"
              ],
              "query": [
                {
                  "key": "comment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "markdown",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "reblog_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tags",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tweet",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Reblogs a post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6978711-51a2-49e5-9efe-cbe2e661f4a0"
            }
          ]
        },
        {
          "id": "0bef1b93-8fa1-4f10-9097-990ceacf6c15",
          "name": "blog.base_hostname.post.delete.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/post/delete"
              ],
              "query": [
                {
                  "key": "id",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "103fcc01-33a0-42fb-b0dd-679691bc7103"
            }
          ]
        }
      ]
    }
  ]
}