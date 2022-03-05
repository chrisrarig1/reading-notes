# Django Forms

## HTML Form

- This will be a HTML form with one or more field on a web page
- Using `<form>` HTML tag we will create the element with an `action` and a `method`
- The form will contain a `<input>` tag with a `type` distinction depending on the data
- Code:

```
<form action="/team_name_url/" method="post">
    <label for="team_name">Enter name: </label>
    <input id="team_name" type="text" name="name_field" value="Default name for team.">
    <input type="submit" value="OK">
</form>
```

- *Action*: This is the URL or resource where the data will be sent
- *Method*: This will either be `post` or `get` depending on whether or not the info is new or you are updating

## Django Form Process

1. Display the default form requested by user
2. Receive data from a submit
3. Clean and validate data
4. If data is invalid redisplay form with error handling
5. If all data is valid perform required actions
6. Once complete redirect user to another page

## Error Handling

- This is done by developing functions inside the class using a if statement for data comparison and `raise ValidationError`

## URL Config

- This is very similar to adding a regular URL, however identifying the specific data item will be necessary for updating or deleting.

- Code:

```
urlpatterns += [
    path('data/create/', views.DataCreate.as_view(), name='data-create'),
    path('data/<int:pk>/update/', views.DataUpdate.as_view(), name='data-update'),
    path('data/<int:pk>/delete/', views.DataDelete.as_view(), name='data-delete'),
]
```

# Django Forms

- [Using Models](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models#summary)