# The Social Network
### A Back-End System for a Social Media Application
![MIT License badge](https://img.shields.io/badge/license-MIT_License-green)

![the-social-network-demo](https://user-images.githubusercontent.com/79285555/134801587-85d50485-23a9-459b-a7d5-a3367d9ebb00.gif)


<p> ---------------------------------------- </p>

Database and API calls written using MongoDB.

[Node.js](https://nodejs.org/en/) is used for as the runtime engine.

The [Mongoose](https://mongoosejs.com/) and [Express](https://expressjs.com/) node packages are used.

## Description
A user may create and manage their business database. The database allows for viewing all departments, roles, or employee list. One may also add a new department, role or employee, as well as update a current employee.

## Table of Contents
* [Installation](#installation)
* [Usage](#usage)
* [Testing](#testing)
* [License](#license)
* [Contributing](#contributing)
* [Questions](#questions)
* [Acknowledgmenets](#Acknowledgments)

## Installation
*THIS DATABASE USES MONGODB AND NODE JS. PLEASE MAKE SURE BOTH ARE INSTALLED ON YOUR MACHINE*

- download or clone application
- open terminal in application root directory
- enter,`npm i`
- *for seeding data into database enter, source db/seeds.sql
- enter,  \quit

- watch [video tutorial](https://drive.google.com/file/d/1HBElkQdgQxMrk20BcEzHFySapOMfL7aq/view?usp=sharing) for in depth installation and usage

## Usage

```bash
npm start
```

## License
MIT License

## Testing
For testing API Routes, [Insomnia CORE](https://insomnia.rest/) is highly recommended.

For viewing Database information [MongoDB Compass](https://www.mongodb.com/products/compass) is highly recommeded.

## Routes

### Users
---
- GET Users: .../api/users
- GET Users: .../api/users/:_id
- POST User: .../api/users
```
{
  "username": "Stephanie",
  "email": "stephanie@gmail.com"
}
```
- PUT User: .../api/users/:_id
```
{
  "email": "stephanie02@gmail.com"
}
```
- DEL User: .../api/users/:_id
- POST Friend: .../api/users/:_id/friends/:_id
*.../api/users/{user-being-added-to}friends/{user-being-added-as-friend}*
- DEL Friend: .../api/users/:_id/friends/:_id
- *.../api/users/{user-being-edited-to}friends/{user-being-removed-as-friend}*


### Thoughts
---
- GET Thoughts: .../api/thoughts
- GET Thought: .../api/thoughts/:_id
- POST Thought: .../api/thought
```
{
  "thoughtText": "Here's a cool thought...",
	"username": "Manuel"
}
```
- PUT Thought: .../api/thoughts/:id
```
{
  "thoughtText": "Here's another cool thought..."
}
```
- DEL Thought: .../api/thoughts/:_id
- POST Reaction: .../api/thoughts/:_id/reactions
```
{
	"reactionBody": "LOVE",
	"username": "toto"
}
```
DEL Reaction: .../api/thoughts/:_id/reactions/:_id
    
Copyright (c) 2021 Anthony Pena

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation fil (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge,publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so,subject to the following conditions:
            
The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
            
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Version History
    
* 0.1
    * Initial Release
    * * See [commit change](https://github.com/anthonypena97/the-social-network/commits/main) or See [release history](https://github.com/anthonypena97/the-social-network/releases)

## Contributing
Please refer to the [Contributor Covenenant](https://www.contributor-covenant.org/) for guidelines on contributing on this project.

## Questions
For any inquiries or questions, please contact Anthony Pena via:
* GitHub: [anthonypena97](https://github.com/anthonypena97)
* Email: <anthony.e.p3na@gmail.com>
