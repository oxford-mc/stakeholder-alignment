
<!-- PROJECT LOGO -->
<br />
<div align="center">
    <img src="images/oxford_logo.png" alt="OxfordLogo" width="150" height="150">

  <h3 align="center">Universal Digital Identity Stakeholder Alignment: Context-Layered RAG Architectures for Ecosystem-Aware AI</h3>

  <p align="center">
    A repository with reproducibility package to accompany the published article
    <br />

  </p>
</div>



<!-- ABOUT THE PROJECT -->
## About The Project

<p>A universal approach to managing a person's digital identity may be the single most important advancement to the Internet since its inception, promising the seamless flow of information, averting cybercrime, eliminating login credentials, and restoring privacy and trust through greater control of one's identity online. However, this advancement brings significant risks, especially regarding personal privacy. It demands the meticulous development of digital identity infrastructure that balances robust data security measures with ethical handling of sensitive information, thereby safeguarding against misuse and unauthorised access. Currently, a consolidated vision for digital identity implementation remains unresolved, and aligning the different stakeholders' motives and expectations is a challenging task. This article reviews and analyses the perspectives and expectations of the four key stakeholder groups - government, business, academia and consumers - regarding a digital identity ecosystem, aiming to increase trust in an eventual design framework.</p>p>

<!-- Use the `BLANK_README.md` to get started.-->

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites
The following prerequistes are required:
1. [Jupyter notebook](https://jupyter.org/)
2. [Python](https://www.python.org/)
3. Python packages: </br><img src="images/packages.png" alt="PythonPackages">


<!-- USAGE EXAMPLES -->
## Usage

In this section we will outline key commands used for the analysis. Note that more comments are available in the notebook itself

### Patent Analysis Notebook
1. Output Patent Leaders </br>
   The following command will output the top 12 entities by patent count over the given dataframe
   ```sh
   output_leaders(wd)
   ```
   <img src="images/leaders.png" alt="Leaders">
2. Display Entity </br>
   This code will display patent counts for the entire dataset, period 1996-2020 and post 2020. In addition it will output the first and last patents within the dataframe
   ```sh
   display_entity(wdfull, "Diebold", [], [])
   ```
   <img src="images/display1.png" alt="Display1">
3. Display Entity with Keywords </br>
   This code will display patent count metrics for each of the provided key term search words
   ```sh
   display_entity(wdfull, "Diebold", ["privacy","trust"], [])
   ```
   <img src="images/display2.png" alt="Display2">
4. Display Entity with Additional Ranges </br>
This code will allow you to specify a subrange e.g. in this case years that Kim Cameron was on staff
   ```sh
   display_entity(wdfull, "Microsoft", ["transaction", "game", "privacy", "trust"], [("Kim Cameron", 1999, 2011, [])])
   ```
    <img src="images/display3.png" alt="Display3">
5. Output Patents for Entity </br>
   This code will output a list of patents with patent hyperlinks by entity name
   ```sh
   print_all_patents(wdfull, "Microsoft")
   ```
   <img src="images/display_patent.png" alt="Display_Patent">
### Patent Modeling Notebook
1. Model Keywords </br>
This code will output base statistics for a search term including percentage movement, mean, std, error and will also output a chart with trend over time
   ```sh
   selected_words = {'certificate','storage','privacy','communication','encryption'}  # Example set of words
   ```
   ```sh
   colors = generate_dark_colors(len(selected_words))
   ```
   ```sh
   plot_graph(selected_words, 'TF-IDF','Security',3, -0.00002)
   ```
   <img src="images/stat1.png" alt="Stat1">
   <img src="images/sc3.png" alt="SC3">
<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Matthew Comb - matthew.comb@linacre.ox.ac.uk

Project Link: [https://github.com/oxford-mc/patent-mining](https://github.com/oxford-mc/patent-mining)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Commonwealth Scholarship Commission in the UK](https://cscuk.fcdo.gov.uk/)
* [Department of Computer Science, University of Oxford](https://www.cs.ox.ac.uk/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
