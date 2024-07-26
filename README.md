<div id="top"></div>

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]


<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/Playtronica/Touchme">
    <img src="static/logo.png" alt="Logo" width="100">
  </a>

<h3 align="center">Touchme</h3>

  <p align="center">
    BODY IS AN INSTRUMENT
    <br />
    <a href="https://github.com/Playtronica/Touchme"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://youtu.be/pB5YI5oH6zg">View Demo</a>
    ·
    <a href="https://github.com/Playtronica/Touchme/issues">Report Bug</a>
    ·
    <a href="https://github.com/Playtronica/Touchme/issues">Request Feature</a>
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
    <li><a href="#contributing">Contributing</li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]](https://example.com)


Turn human skin, water, or flowers into a musical instrument with TouchMe. Play alone or with your friends!

As the area of touch and intensity changes, the sound changes too.

Ready to get started? You need a computer, tablet, or smartphone, as well as a TouchMe device and objects that can conduct electricity. 

Just open any [online synth](https://synth.[laytronica.com/), and you're ready to play!  No noticeable latency, [TouchMe](https://shop.playtronica.com/products/touchme) reacts just as any other midi controller. 

### Key Features/ Functionality

Measure resistance change between two contacts and transposes it into MIDI (musical notation) data sent to computers or smartphones via USB.


<!-- Here's a blank template to get started: To avoid retyping too much info. Do a search and replace with your text editor for the following: `Playtronica`, `Touchme`, `twitter_handle`, `linkedin_username`, `email_client`, `email`, `project_title`, `project_description` -->

<p align="right">(<a href="#top">back to top</a>)</p>



### Built With

* [Docker](https://www.docker.com/)
* [Raspberry Pi Pico SDK](https://github.com/raspberrypi/pico-sdk)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started


### Prerequisites

Install docker, example for Ubuntu 20.04

```sh
sudo apt update
sudo apt install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
sudo apt update
sudo apt install make docker-ce 
```

### Build and flash with docker (Recomended way)

1. Clone the repo
   ```sh
   git clone https://github.com/Playtronica/Touchme.git
   ```
2. Setup build image
   ```sh
   make build_image
   ```
3. Build binary
   ```sh
   make build
   ```
4. Boot touchme in bootloader mode
- * Span the two boot contacts with something metal
- * Plug in USB cable
- * Will appear mass storage device

5. Copy `touchme.uf2` from `output` dir to touchme mass storage device  
  Example:
    ```sh
    cp output/touchme.uf2 /media/user/RPI-RP2
    ```

<p align="right">(<a href="#top">back to top</a>)</p>





<!-- ROADMAP -->
<!-- ## Roadmap

- [ ] Feature 1
- [ ] Feature 2
- [ ] Feature 3
    - [ ] Nested Feature

See the [open issues](https://github.com/Playtronica/Touchme/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#top">back to top</a>)</p> -->



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



<!-- LICENSE -->
## License
 TODO Add license

<!-- Distributed under the MIT License. See `LICENSE.txt` for more information. -->

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

* Project Link: [https://github.com/Playtronica/Touchme](https://github.com/Playtronica/Touchme)
* Our website: [https://playtronica.com/](https://laytronica.com/)

### Social media
* [Facebook](https://www.facebook.com/playtronica)
* [Instagram](http://instagram.com/playtronica)
* [Twitter](https://twitter.com/playtronica)
* [Youtube](https://www.youtube.com/playtronica)


<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
<!-- ## Acknowledgments

* []()
* []()
* []()

<p align="right">(<a href="#top">back to top</a>)</p> -->



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/Playtronica/Touchme.svg?style=for-the-badge
[contributors-url]: https://github.com/Playtronica/Touchme/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Playtronica/Touchme.svg?style=for-the-badge
[forks-url]: https://github.com/Playtronica/Touchme/network/members
[stars-shield]: https://img.shields.io/github/stars/Playtronica/Touchme.svg?style=for-the-badge
[stars-url]: https://github.com/Playtronica/Touchme/stargazers
[issues-shield]: https://img.shields.io/github/issues/Playtronica/Touchme.svg?style=for-the-badge
[issues-url]: https://github.com/Playtronica/Touchme/issues
[license-shield]: https://img.shields.io/github/license/Playtronica/Touchme.svg?style=for-the-badge
[license-url]: https://github.com/Playtronica/Touchme/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[product-screenshot]: static/touchme.png