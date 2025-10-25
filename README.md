# GraphQL Lab

A learning project to explore GraphQL fundamentals using Apollo Server and Node.js. This simple API demonstrates basic CRUD operations with user management.

## About

This project is part of my journey learning GraphQL. It implements a basic server with queries and mutations to create and list users, serving as a foundation for understanding GraphQL concepts.

## Features

- ✨ Create new users with mutations
- 📋 Query all users
- 🚀 Apollo Server implementation
- 💾 In-memory data storage

## Prerequisites

- Node.js (v14 or higher)
- npm or yarn

## Installation

Clone the repository and install dependencies:

```bash
git clone <your-repository-url>
cd graphql-lab
npm install
```

## Running the Server

Start the development server:

```bash
npm start
```

The GraphQL server will be available at: **http://localhost:4000/**

## API Usage

### Create a User

Use this mutation to create a new user:

```graphql
mutation CreateUser($name: String!) {
  createUser(name: $name) {
    id
    name
  }
}
```

**Variables:**
```json
{
  "name": "John Doe"
}
```

### List All Users

Query to fetch all users:

```graphql
query Users {
  users {
    id
    name
  }
}
```

## Technologies Used

- [Apollo Server](https://www.apollographql.com/docs/apollo-server/) - GraphQL server
- [GraphQL](https://graphql.org/) - Query language for APIs
- [Node.js](https://nodejs.org/) - JavaScript runtime

## Learning Resources

- [GraphQL Official Documentation](https://graphql.org/learn/)
- [Apollo Server Documentation](https://www.apollographql.com/docs/apollo-server/)
- [How to GraphQL](https://www.howtographql.com/)

## Next Steps

Future improvements planned for this learning project:

- [ ] Add update and delete mutations
- [ ] Implement data persistence with a database
- [ ] Add authentication and authorization
- [ ] Create more complex schema relationships
- [ ] Add input validation
- [ ] Write unit tests

## License

This is a learning project and is open for educational purposes.

## Author

Created while learning GraphQL concepts and best practices.

---

**Happy coding! 🚀**