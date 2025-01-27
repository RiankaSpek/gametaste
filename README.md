
# GameTaste 🎮

GameTaste is a cutting-edge game review project that offers users an intuitive and user-friendly platform to share their opinions on their favorite games. Developed using a custom framework, this project leverages the power of IGDB API and TailwindCSS to provide an unparalleled experience to gamers around the world.

One of the standout features of GameTaste is its dark mode, which makes it easy on the eyes for users who prefer a more subdued color palette. Additionally, GameTaste provides users with the ability to create their own profile, complete with a bio and profile picture. This personalized touch allows users to showcase their gaming interests and connect with like-minded individuals.

Another great feature of GameTaste is the ability to review any game. Whether it's an old classic or a brand new release, users can share their thoughts and experiences with the gaming community. To make their reviews stand out, users can use markdown to style their content and add flair to their writing.
## Authors

- [@danylayasmin](https://github.com/danylayasmin)
- [@RiankaSpek](https://github.com/RiankaSpek)
- [@rico-vz](https://github.com/rico-vz)
- [@Dylan-Kuiper](https://github.com/Dylan-Kuiper)
## Features

- Dark mode
- User profile with bio & profile picture
- Review any game
- Use markdown to style your reviews
- Home page; currently trending games
- Review feed
## Installation

#### Requirements:
- PHP 7.4+
- MySQL
- Nginx/Apache
- Git
- IGDB API Key

1. Clone this repository:
    ```bash 
    git clone git@github.com:rico-vz/gametaste.git
    ```

2. Update/Install all Composer dependencies:
    ```bash 
    composer update
    ```

3. Configure your Nginx or Apache to serve from ./public.

4. In the case of using Nginx, apply the following rewrite rule:
    ```conf
    location / {
      if (!-e $request_filename){
        rewrite ^/(.*)$ /index.php?controller=$1 last;
      }
    }
    ```

5. Go to the BaseController and change the following to your own credentials:
    ```
    $this->client_ID = "YOUR_CLIENT_ID";
    $this->access_token = "YOUR_ACCESS_TOKEN";
    ```


6. Go to index.php and change the database credentials to yours.

## Screenshots

![GameTaste Homepage](https://i.imgur.com/1r7uUVg.png)
![GameTaste Homepage](https://i.imgur.com/fGP80zs.png)
![GameTaste Review Page](https://i.imgur.com/n5XxIj2.png)