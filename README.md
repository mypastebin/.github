# MyPastebin Project

**MyPastebin** is a personal project designed as a simpler, educational version of [Pastebin](https://pastebin.com/), where users can store and share text snippets. Additionally, it includes a custom **hash generator** service that pre-generates unique hashes for quicker access when creating posts. The project is built using **Spring Boot**, **MySQL**, **Redis**, and **Docker**.

## Features

- **Paste Management**: Users can create, retrieve, and delete text-based "pastes" that are stored in a MySQL database.
- **Expiration Dates**: Each paste has an optional expiration date, after which it becomes inaccessible.
- **Hash Generator**: The project includes a service that generates unique hashes to be used as identifiers for each paste.
- **Redis Queue for Pre-generated Hashes**: The hash generator service uses Redis to store pre-generated hashes, optimizing performance by quickly delivering a hash without needing to generate it on the fly.
- **RESTful API**: The application exposes a REST API to handle all operations, including managing pastes and generating hashes.
- **Google Cloud Storage Integration**: For added functionality, the API integrates with Google Cloud Storage for optional cloud storage of pastes.
