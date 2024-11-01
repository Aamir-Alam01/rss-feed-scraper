# RSS Feed Scraper Server

RSSAGG is a Go-based HTTP server that scrapes RSS feeds from websites, stores feed data in a PostgreSQL database, and provides an API to retrieve and manage the feeds and their posts.

## Features

- Scrapes posts from multiple RSS feeds and stores them in a PostgreSQL database.
- Allows clients to retrieve RSS feed posts via a RESTful API.
- Designed to be easy to deploy and configure.
- Written in Go for performance and simplicity.

## Prerequisites

- Go (v1.16 or newer)
- PostgreSQL (v13 or newer)

## Clone the repository

``` bash
 git clone https://github.com/Aamir-Alam01/rss-feed-scraper
cd rss-feed-scraper
```

### Configuration

Rename `.env.example` to `.env` and set your environment variables:
```bash
DB_URL=postgres://user:yourpassword@localhost:5432/rssagg?sslmode=disable

PORT=8080
```

### Build and Run
```bash
go build -o rag-server 
./rag-server

```
Your server should now be running on http://localhost:8080.