# 🐾 Pet Society
Pet Society is a social network designed for pet lovers to share photos of their pets and create a vibrant community. 
Users can interact through likes, comments, and follow their favorite pet enthusiasts, fostering a passionate community of pet lovers.
![image](https://github.com/user-attachments/assets/4b7da9d8-1d61-4efc-a544-c4481171f5c1)

**More info about EndPoints here:** [API Documentation](http://localhost:8080/swagger-ui/index.html)

## Table of Contents :bookmark_tabs:
| Index | Title |
|-------|-------|
| 1     | [Project Description](#-project-description) |
| 2     | [Features](#-features) |
| 3     | [Technologies Used](#-technologies-used) |
| 4     | [Getting Started](#-getting-started) |
| 5     | [Prerequisites](#-prerequisites) |
| 6     | [Installation](#-installation) |
| 7     | [Built With](#-built-with) |
| 8     | [Contributing](#-contributing) |
| 9     | [Wiki](#-wiki) |
| 10    | [Versioning](#-versioning) |
| 11    | [Authors](#-authors) |
| 12    | [License](#-license) |
| 13    | [Acknowledgments](#-acknowledgments) |
| 14    | [API Documentation](#-api-documentation) |


## 🌟 Features
- **User Registration:** Allow pet lovers to create unique and verified accounts.
- **Post Sharing:** Users can share their pet photos through interactive posts.
- **Exploration and Recommendations:** Discover new pets and experiences through personalized recommendations. Whether you're looking for new friends for your furry companion or inspiration for pet care, our exploration feature has got you covered!

## 💻 Technologies Used
- **Backend:** Java Spring Boot
- **Database:** MySQL
- **Frontend:** JavaScript, CSS, HTML

## 🚀 Getting Started
### 🌐 Installation Instructions
The project is available on GitHub. You can get a copy of the project in two ways:

1. **Fork the repository:**
   - Go to the project's repository on GitHub.
   - Click on the "Fork" button in the upper right corner.
   - This will create a copy of the repository in your GitHub account.

2. **Download the copy:**
   - Go to the project's repository on GitHub.
   - Click on the "Code" button and select "Download ZIP".
   - Extract the files from the downloaded ZIP on your local machine.

Once you have a copy of the project, you can follow the specific installation and configuration instructions included in the repository.

## 🚀 Deployment
See Deployment for information on how to deploy the project.

## 📋 Prerequisites
Things you need to install the software and how to install them:
- **Java:** You need to have Java installed on your machine. You can download and install it from [here](https://www.java.com/en/download/).
- **Spring Boot Security:** Our project uses Spring Boot Security. Make sure to follow the specific configuration in the [Spring Boot documentation](https://spring.io/projects/spring-boot).
- **Browser:** A modern web browser to access the project's interface.
- **NetBeans:** Use NetBeans IDE for development. You can download it from [here](https://netbeans.apache.org/).
- **JavaScript:** Ensure you have JavaScript enabled in your browser.

## 🚀 Installation
1. **Clone the repository:** Clone the project repository from GitHub to your local machine.
2. **Install Java:** Make sure you have Java installed on your machine.
3. **Configure Spring Boot:** Our project uses Spring Boot Security.
4. **Configure NetBeans:** Set up NetBeans IDE for development.
5. **Install JavaScript dependencies:** Ensure your browser has JavaScript enabled.

## 🛠️ Built With

- **Maven:** Dependency management.
- **Java Spring Boot:** Backend framework.
- **MySQL:** Database management system.
- **JavaScript, CSS, HTML:** Frontend technologies.

---

## 📚 API Documentation
### Overview
This API provides endpoints for user interaction, allowing for managing user profiles, posts, comments, likes, followers, and notifications 
in a pet-themed social network.

**Base URL:** `http://localhost:8080`

### **API Documentation Table of Contents**

#### **Login Controller**
- **POST** `/register`
- **POST** `/login`

#### **User Controller**
- **POST** `/api/user/create`
- **PATCH** `/api/user/update/photo/{email}`
- **PATCH** `/api/user/update/password/{email}`
- **PATCH** `/api/user/update/biography/{email}`
- **PATCH** `/api/user/update/all/{email}`
- **PATCH** `/api/user/update/active/{email}`
- **GET** `/api/user/{email}`
- **GET** `/api/user/notfollowed/{email}`
- **GET** `/api/user/all`

#### **Post Controller**
- **POST** `/api/post/create`
- **PATCH** `/api/post/update/description/{id}`
- **GET** `/api/post/followed/{email}`
- **GET** `/api/post/all`
- **GET** `/api/post/all/{email}`
- **DELETE** `/api/post/delete/{id}`

#### **Likes Controller**
- **POST** `/api/likes/create/likepost`
- **POST** `/api/likes/create/likecomment`
- **GET** `/api/likes/all/likepost/{idPost}`
- **GET** `/api/likes/all/likecomment/{idComment}`
- **DELETE** `/api/likes/delete/likepost/{id}`
- **DELETE** `/api/likes/delete/likecomment/{id}`

#### **Follower Group Controller**
- **POST** `/api/follow/create/{emailFollower}`
- **GET** `/api/follow/all/followers/{emailFollowed}`
- **GET** `/api/follow/all/followeds/{emailFollower}`
- **DELETE** `/api/follow/delete/{emailFollower}`

#### **Comment Controller**
- **POST** `/api/comment/create`
- **PATCH** `/api/comment/update/content/{id}`
- **GET** `/api/comment/all/{postId}`
- **DELETE** `/api/comment/delete/{commenttId}`

#### **Notify Controller**
- **PATCH** `/api/notify/update/opened/{idNotification}`
- **GET** `/api/notify/all/{email}`
- **DELETE** `/api/notify/delete/{follow}`

#### **Search User Controller**
- **GET** `/api/search/searchUsers`

## ✒️ Authors
- **Frontend Developer:** Jhoan Sebastian Diaz Ardila
- **Backend Developer:** Maria Camila Diaz Toledo
