[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/HideyoshiNakazone/hideyoshi.com">
    <img src="https://drive.google.com/uc?export=view&id=1ka1kTMcloX_wjAlKLET9VoaRTyRuGmxQ" width="100" height="100" allow="autoplay"\>
  </a>

  <h3 align="center">Hideyoshi - Web Porfolio</h3>

  <p align="center">
    A awesome web portfolio built with Angular and Spring Boot
    <br />
    <a href="https://hideyoshi.com.br">View</a>
    ·
    <a href="https://github.com/HideyoshiNakazone/hideyoshi.com/issues">Report Bug</a>
    ·
    <a href="https://github.com/HideyoshiNakazone/hideyoshi.com/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

This project is the result of my curiosity of web applications and the necessity for a portfolio, which results in this awesome web portfolio. Built with Angular and Spring and deployed in kubernetes this project uses the best technologies available.


<p align="right">(<a href="#top">back to top</a>)</p>


### Built With

This project is composed of the following technologies:

* Frontend: [Angular](https://angular.io/) (Currently using AngularJS but Angular2+ on development);
* Backend: [Spring Boot](http://spring.io/)
* Deployment: [kubernetes](https://kubernetes.io/pt-br/)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

At the moment you have several options to run the application, you can run each individual projects or you can run the full application using the deployment with minikube.

### Prerequisites

* Stand Alone Deployment:

    - npm
        ```sh
        npm install npm@latest -g
        ```
    
    - Docker-compose (Linux)
        ```
        sudo curl -L "https://github.com/docker/compose/releases/download/1.26.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
        sudo chmod +x /usr/local/bin/docker-compose
        ```

* Full Deployment:

    - [Installing kvm2 on Ubuntu](https://ubuntu.com/blog/kvm-hyphervisor)
    
    - minikube (Linux)
        ```
        curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
        sudo install minikube-linux-amd64 /usr/local/bin/minikube
        ```

### Installation

* Stand Alone Deployment:

    This option requires you to set the environment variable, follow the exemple files.
    After setting the environment variable, create a directory and start each package:

    ```
    mkdir hideyoshi-portfolio
    cd ./hideyoshi-portfolio
    ```

    - Frontend:

        ```
        git clone https://github.com/HideyoshiNakazone/frontend-hideyoshi.com.git
        cd ./frontend-hideyoshi.com
        npm install .
        node ./serv.js
        cd ..
        ```

    - Backend:

        ```
        git clone https://github.com/HideyoshiNakazone/backend-hideyoshi.com.git
        cd ./backend-hideyoshi.com
        mvn spring-boot:run
        cd ..
        ```

* Full Deployment:

    Sets the entire environment using minikube

    ```
    git clone https://github.com/HideyoshiNakazone/infra-hideyoshi.com.git
    cd ./infra-hideyoshi.com
    ./deploy.sh --test
    ```

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- LICENSE -->
## License

Distributed under the GPLv3 License. See ```LICENSE``` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- CONTACT -->
## Contact

Vitor Hideyoshi - [@NakazoneVitor](https://twitter.com/NakazoneVitor) - vitor.h.n.batista@gmail.com

Project Link: [https://github.com/HideyoshiNakazone/hideyoshi.com](https://github.com/HideyoshiNakazone/hideyoshi.com)


<p align="right">(<a href="#top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/HideyoshiNakazone/hideyoshi.com.svg?style=for-the-badge
[contributors-url]: https://github.com/HideyoshiNakazone/hideyoshi.com/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/HideyoshiNakazone/hideyoshi.com.svg?style=for-the-badge
[forks-url]: https://github.com/HideyoshiNakazone/hideyoshi.com/network/members
[stars-shield]: https://img.shields.io/github/stars/HideyoshiNakazone/hideyoshi.com.svg?style=for-the-badge
[stars-url]: https://github.com/HideyoshiNakazone/hideyoshi.com/stargazers
[issues-shield]: https://img.shields.io/github/issues/HideyoshiNakazone/hideyoshi.com.svg?style=for-the-badge
[issues-url]: https://github.com/HideyoshiNakazone/hideyoshi.com/issues
[license-shield]: https://img.shields.io/github/license/HideyoshiNakazone/hideyoshi.com.svg?style=for-the-badge
[license-url]: https://github.com/HideyoshiNakazone/hideyoshi.com/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/vitor-hideyoshi-nakazone-batista/
