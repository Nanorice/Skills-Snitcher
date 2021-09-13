<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Thanks again! Now go create something AMAZING! :D
-->



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
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/Nanorice/Skills-Snitcher">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Skill-Snitcher</h3>

  <p align="center">
    A NLP project in extracting and analysing skill entities from job posts.
    <br />
    <a href="https://github.com/Nanorice/Skills-Snitcher"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/Nanorice/Skills-Snitcher">View Demo</a>
    ·
    <a href="https://github.com/Nanorice/Skills-Snitcher/issues">Report Bug</a>
    ·
    <a href="https://github.com/Nanorice/Skills-Snitcher/issues">Request Feature</a>
  </p>
</p>



<!-- TABLE OF CONTENTS -->
<details open="open">
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
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

![Product Name Screen Shot][pca_occupation.png]

This project is oriented around the skills requirement aspect of job postings on the online recruitment platforms. 

The coding contains sections specializing and sequencing on the following tasks: 
* acquire job posting data through scraping indeed.com by specifying predefined search criteria
* parsing the scraped textual into job Common Schema
* predict the occupation classifier based on texts of job descriptions through means of doc2vec embeddings (which is pre-trained based on previously concatenated dataset)
* extracting skill entities disambiguated using occupation classification coded (SOC)
* embedding the previously extracted into normalized vectors that could be then visualized through either t-SNE or PCA to showcase the overlapping and differences. 

The formulated pipeline for processing of textual skill entities provides a ready-to-use tool for researchers in labour markets to address problems such as evolution of job titles, discrepancies of skill requirements between different industries, lifecycle of a job inside an organization and identify what crucial skills are needed for promotions and sustainability and potentially many more.

### Built With

This section should list any major frameworks that you built your project using. Leave any add-ons/plugins for the acknowledgements section. Here are a few examples.
* [skills-ml](https://github.com/workforce-data-initiative/skills-ml)
* [Bootstrap](https://getbootstrap.com)



<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

This project is dependent on the following requirements at the time of writing.

name: skills_ml
channels:
  - conda-forge
  - defaults
dependencies:
  - absl-py=0.9.0=py36_0
  - appnope=0.1.0=py36hf537a9a_0
  - astor=0.8.1=pyh9f0ad1d_0
  - attrs=19.3.0=py_0
  - backcall=0.2.0=py_0
  - blas=1.0=mkl
  - bleach=3.1.5=py_0
  - bokeh=2.1.1=py36_0
  - c-ares=1.16.1=haf1e3a3_0
  - ca-certificates=2020.6.24=0
  - certifi=2020.6.20=py36_0
  - cycler=0.10.0=py36hfc81398_0
  - dbus=1.13.16=h18a8e69_0
  - decorator=4.4.2=py_0
  - defusedxml=0.6.0=py_0
  - entrypoints=0.3=py36_0
  - expat=2.2.9=hb1e8313_2
  - freetype=2.10.2=ha233b18_0
  - gast=0.3.3=py_0
  - gettext=0.19.8.1=hb0f4f8b_2
  - git=2.23.0=pl526h6951d83_0
  - glib=2.65.0=hc5f4afa_0
  - google-pasta=0.2.0=pyh8c360ce_0
  - grpcio=1.30.0=py36h7c1f37e_0
  - h5py=2.10.0=nompi_py36h106b333_102
  - hdf5=1.10.5=nompi_h0cbb7df_1103
  - icu=58.2=h0a44026_3
  - importlib-metadata=1.7.0=py36_0
  - importlib_metadata=1.7.0=0
  - intel-openmp=2019.4=233
  - ipykernel=5.3.4=py36h5ca1d4c_0
  - ipython=7.16.1=py36h5ca1d4c_0
  - ipython_genutils=0.2.0=py36_0
  - ipywidgets=7.5.1=py_0
  - jedi=0.17.1=py36_0
  - jinja2=2.11.2=py_0
  - jpeg=9b=he5867d9_2
  - jsonschema=3.2.0=py36_0
  - jupyter=1.0.0=py36_7
  - jupyter_client=6.1.6=py_0
  - jupyter_console=6.1.0=py_0
  - jupyter_contrib_core=0.3.3=py_2
  - jupyter_contrib_nbextensions=0.5.1=py36_0
  - jupyter_core=4.6.3=py36_0
  - jupyter_highlight_selected_word=0.2.0=py36_1000
  - jupyter_latex_envs=1.4.4=py36_1000
  - jupyter_nbextensions_configurator=0.4.1=py36h9f0ad1d_1
  - keras-applications=1.0.8=py_1
  - keras-preprocessing=1.1.0=py_0
  - kiwisolver=1.2.0=py36h04f5b5a_0
  - krb5=1.18.2=h75d18d8_0
  - lcms2=2.11=h92f6f08_0
  - libcurl=7.71.1=h8a08a2b_1
  - libcxx=10.0.0=1
  - libedit=3.1.20191231=h1de35cc_1
  - libffi=3.3=hb1e8313_2
  - libgfortran=3.0.1=0
  - libiconv=1.16=h1de35cc_0
  - libpng=1.6.37=ha441bb4_0
  - libprotobuf=3.12.3=hab81aa3_2
  - libsodium=1.0.18=h1de35cc_0
  - libssh2=1.9.0=ha12b0ac_1
  - libtiff=4.1.0=hcb84e12_1
  - libxml2=2.9.10=h3b9e6c8_1
  - libxslt=1.1.34=h83b36ba_0
  - lz4-c=1.9.2=hb1e8313_1
  - markdown=3.2.2=py_0
  - markupsafe=1.1.1=py36h1de35cc_0
  - matplotlib=3.2.2=0
  - matplotlib-base=3.2.2=py36h5670ca0_0
  - mistune=0.8.4=py36h1de35cc_0
  - mkl=2019.4=233
  - mkl-service=2.3.0=py36hfbe908c_0
  - mkl_fft=1.1.0=py36hc64f4ea_0
  - mkl_random=1.1.1=py36h959d312_0
  - nbconvert=5.6.1=py36_0
  - nbformat=5.0.7=py_0
  - ncurses=6.2=h0a44026_1
  - notebook=6.0.3=py36_0
  - numpy=1.19.1=py36h3b9f5b6_0
  - numpy-base=1.19.1=py36hcfb5961_0
  - olefile=0.46=py36_0
  - openssl=1.1.1g=h1de35cc_0
  - packaging=20.4=py_0
  - pandoc=2.10=0
  - pandocfilters=1.4.2=py36_1
  - parso=0.7.0=py_0
  - pcre=8.44=hb1e8313_0
  - perl=5.26.2=h4e221da_0
  - pexpect=4.8.0=py36_0
  - pickleshare=0.7.5=py36_0
  - pillow=7.2.0=py36ha54b6ba_0
  - pip=20.1.1=py36_1
  - prometheus_client=0.8.0=py_0
  - prompt-toolkit=3.0.5=py_0
  - prompt_toolkit=3.0.5=0
  - protobuf=3.12.3=py36h0130604_0
  - ptyprocess=0.6.0=py36_0
  - pygments=2.6.1=py_0
  - pyparsing=2.4.7=py_0
  - pyqt=5.9.2=py36h655552a_2
  - pyrsistent=0.16.0=py36h1de35cc_0
  - python=3.6.10=hf48f09d_2
  - python-dateutil=2.8.1=py_0
  - python_abi=3.6=1_cp36m
  - pytz=2020.1=py_0
  - pyyaml=5.3.1=py36h37b9a7d_0
  - pyzmq=19.0.1=py36hb1e8313_1
  - qt=5.9.7=h468cd18_1
  - qtconsole=4.7.5=py_0
  - qtpy=1.9.0=py_0
  - readline=8.0=h1de35cc_0
  - seaborn=0.10.1=py_0
  - send2trash=1.5.0=py36_0
  - setuptools=49.2.0=py36_0
  - sip=4.19.8=py36h0a44026_0
  - six=1.15.0=py_0
  - sqlite=3.32.3=hffcf06c_0
  - tensorboard=1.14.0=py36_0
  - tensorflow=1.14.0=hcba10bf_0
  - tensorflow-base=1.14.0=py36h9f0ad1d_0
  - tensorflow-estimator=1.14.0=py36h5ca1d4c_0
  - termcolor=1.1.0=py_2
  - terminado=0.8.3=py36_0
  - testpath=0.4.4=py_0
  - tk=8.6.10=hb0a8c7a_0
  - tornado=6.0.4=py36h1de35cc_1
  - traitlets=4.3.3=py36_0
  - typing_extensions=3.7.4.2=py_0
  - wcwidth=0.2.5=py_0
  - webencodings=0.5.1=py36_1
  - werkzeug=1.0.1=pyh9f0ad1d_0
  - wheel=0.34.2=py36_0
  - widgetsnbextension=3.5.1=py36_0
  - wrapt=1.12.1=py36h37b9a7d_1
  - xz=5.2.5=h1de35cc_0
  - yaml=0.2.5=h0b31af3_0
  - zeromq=4.3.2=hb1e8313_2
  - zipp=3.1.0=py_0
  - zlib=1.2.11=h1de35cc_3
  - zstd=1.4.5=h41d2c2f_0
  - pip:
    - alembic==1.0.2
    - annoy==1.14.0
    - atomicwrites==1.4.0
    - beautifulsoup4==4.9.1
    - boto==2.49.0
    - boto3==1.14.33
    - botocore==1.17.33
    - bs4==0.0.1
    - chardet==3.0.4
    - click==7.1.2
    - click-plugins==1.1.1
    - cligj==0.5.0
    - dickens==1.0.1
    - dill==0.2.8.2
    - docutils==0.15.2
    - elasticsearch==6.3.1
    - filelock==3.0.10
    - fiona==1.8.0
    - future==0.18.2
    - fuzzywuzzy==0.17.0
    - gensim==3.6.0
    - geocoder==1.38.1
    - idna==2.7
    - jellyfish==0.5.6
    - jmespath==0.10.0
    - lxml==4.2.5
    - mako==1.1.3
    - more-itertools==8.4.0
    - multiprocess==0.70.6.1
    - munch==2.5.0
    - nltk==3.2.5
    - pandas==0.23.4
    - pluggy==0.13.1
    - psycopg2==2.7.6.1
    - py==1.9.0
    - pytest==3.10.1
    - python-editor==1.0.4
    - python-graphviz==0.14.1
    - python-levenshtein==0.12.0
    - ratelim==0.1.6
    - requests==2.20.1
    - retrying==1.3.3
    - s3fs==0.1.6
    - s3transfer==0.3.3
    - scikit-learn==0.20.0
    - scipy==1.1.0
    - shapely==1.6.4.post2
    - skills-ml==2.1.0
    - skills-utils==0.4.0
    - smart-open==2.1.0
    - soupsieve==2.0.1
    - sqlalchemy==1.2.14
    - toolz==0.9.0
    - unicodecsv==0.14.1
    - urllib3==1.24.3
    - us==1.0.0



<!-- USAGE EXAMPLES -->
## Usage

The pipeline utilized the functionalities of open-source library Skills-ML to perform the extractions of skill entities with several modifications. The general instruction for usage of this package is demonstrated on the ‘Skill-ml tour’ notebook file. 

The main part of the code is modified into the following notebooks with comments on directions to use, with index representing order to execute. The folder main folder contains three subfolders, code, data and output, each functioning as a referencing path to store data file as well as output charts. The file 04a performs a basic a basic demonstration on addressing the research problem addressed in the vignette 1 in the working paper. In addition, in the requirement folder contains the exported conda environment file.

![Product Name Screen Shot][asset_list.png]

<!-- ROADMAP -->
## Schematics

![Product Name Screen Shot][schematics.jpg]

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.




<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/Nanorice/Skills-Snitcher.svg?style=for-the-badge
[contributors-url]: https://github.com/Nanorice/Skills-Snitcher/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Nanorice/Skills-Snitcher.svg?style=for-the-badge
[forks-url]: https://github.com/Nanorice/Skills-Snitcher/network/members
[stars-shield]: https://img.shields.io/github/stars/Nanorice/Skills-Snitcher.svg?style=for-the-badge
[stars-url]: https://github.com/Nanorice/Skills-Snitcher/stargazers
[issues-shield]: https://img.shields.io/github/issues/Nanorice/Skills-Snitcher.svg?style=for-the-badge
[issues-url]: https://github.com/Nanorice/Skills-Snitcher/issues
[license-shield]: https://img.shields.io/github/license/Nanorice/Skills-Snitcher.svg?style=for-the-badge
[license-url]: https://github.com/Nanorice/Skills-Snitcher/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
