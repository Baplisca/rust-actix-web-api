# rust-actix-web-api

## Usage

git clone this repo in terminal

```
git clone git@github.com:Baplisca/rust-actix-web-api.git
```

run server app

```
cargo run main.rs
```

you can check with curl command

[GET]

```
curl --location --request GET 'localhost:8080/todolist/entries'
```

[POST]

```
curl --location --request POST 'localhost:8080/todolist/entries' \
--header 'Content-Type: application/json' \
--data-raw '{
    "title": "aaa",
    "date": 1111
}'
```

[PUT]

```
curl --location --request PUT 'localhost:8080/todolist/entries/1' \
--header 'Content-Type: application/json' \
--data-raw '{
    "title": "bbbb"
}'
```

[DELETE]

```
curl --location --request DELETE 'localhost:8080/todolist/entries/1'
```

## Language

- rust 1.66.0

## Library

- cargo 1.66.0
- actix-web 4.2.1
- rust-analyzer v0.3.1359
