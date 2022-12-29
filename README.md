# Ruby On Rails

---

USER
Description
Action / URL
Body (if applicable)

Creating user
POST
/users

```
{
    “username” string
    “Password” string
}
```

Login
POST
/login

```
{
    “username” string
    “Password” string
}
```

---

POST
Description
Action / URL
Body (if applicable)

Creating post
POST
/posts

```
{
	“title” string
	“body” string
	“category” string
}
```

Getting all posts
GET
/posts

-

Get specific post
GET
/posts/:post_id

-

Updating specific post
PATCH
/posts/:post_id

```
{
	“title” string
	“body” string
	“category” string
}
```

Deleting specific post
DELETE
/posts/:post_id

---

COMMENT
Description
Action / URL
Body (if applicable)

Creating comment
POST
/comments

```
{
	“body” string
	“post_id” int
}
```

Getting all posts
GET
/comments

-

Get specific post
GET
/comments/:comment_id

-

Getting all comments regarding specific post
GET
/posts/:post_id/comments

-

Updating specific comment
PATCH
/comments/:comment_id

```
{
	“body” string
	“post_id” int
}
```

Deleting specific comment
DELETE
/comments/:comment_id

-
