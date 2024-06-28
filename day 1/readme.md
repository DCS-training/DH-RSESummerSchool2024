# Day 1: 02 July 2024, Edinburgh Future Institute

## Centre for Data Culture and Society

## Schedule
- 08:40-09:10 Registration (Room 1.50)
- 09.10-09:30 Welcome and Introduction (Lucia Michielin & Lisa Otty)
- 09.30-10:30 **Project Deep Dive**: Coding my way out of a box: Achieving emancipation and collaboration through the Digital Humanities (Will Lamb)
- 10:30-11:00 Break
- 11:12:30 **DH&RSE at Edinburgh**: What it means to work as an RSE in the Humanities and Social Sciences College at the University of Edinburgh. Round Table (Ed MacKenzie, Alexis Pister, Evan Morgan)
- 12:30-13:30 Lunch
- 13:30-15:00 **Workshop**: Data visualisation with R (Lucia Michielin, Aislinn Keogh)
- 15:00-15:30 Break
- 15:30-17:00 **Workshop**: Custom data visualisation with D3 (Sarah Schöttler, Aislinn Keogh)
- 17.00 Close

## Speakers

- [Aislinn Keogh](https://aislinnkeogh.github.io/), Centre for Data, Culture & Society
- [Alexis Pister](https://efi.ed.ac.uk/people/alexis-pister/), Edinburgh Future Institute
- [Ed Mackenzie](https://efi.ed.ac.uk/people/ed-mackenzie/), Centre for Data, Culture & Society
- [Evan Morgan](https://www.designinformatics.org/person/evan-morgan/), Design Informatics
- [Lisa Otty](https://efi.ed.ac.uk/people/lisa-otty/), Centre for Data, Culture & Society
- [Lucia Michielin](https://efi.ed.ac.uk/people/lucia-michielin/), Centre for Data, Culture & Society
- [Sarah Schöttler](https://sarahschoettler.com/), Centre for Data, Culture & Society


## Workshop Setting up

### Data Visualisation with R
You can either run the code on your own machine or through Posit (RStudio Online IDE).
Below are the instructions for setting up on Posit or locally.

#### On Posit
1. Go to https://posit.cloud/
2. Signup either via Gmail or GitHub
3. Go on New Project
4. New Project from Git Repository
5. Copy and Paste this repository URL [https://github.com/DCS-training/DH-RSESummerSchool2024/day%1](https://github.com/DCS-training/DH-RSESummerSchool2024/day%1) as the Repository URL
6. The Project directory name will filled in automatically

#### Locally
* R and RStudio are separate downloads and installations. R is the underlying statistical computing environment, but using R alone is no fun. RStudio is a graphical integrated development environment (IDE) that makes
using R much easier and more interactive. You need to install R before you install RStudio. After installing both programs, you will need to install  some specific R packages within RStudio. Follow the instructions below for your operating system, and then follow the instructions to install the needed packages(below)

**Windows**
- If you already have R and RStudio installed
* Open RStudio, and click on "Help" > "Check for updates". If a new version is available, quit RStudio, and download the latest version for RStudio.
* To check which version of R you are using, start RStudio and the first thing that appears in the console indicates the version of R you are running. Alternatively, you can type `sessionInfo()`, which will also display which version of R you are running. Go on the [CRAN website](https://cran.r-project.org/bin/windows/base/) and check whether a more recent version is available. If so, please download and install it. You can [check here](https://cran.r-project.org/bin/windows/base/rw-FAQ.html#How-do-I-UNinstall-R_003f) for more information on how to remove old versions from your system if you wish to do so.
- If you don't have R and RStudio installed
* Download R from the [CRAN website](https://cran.r-project.org/bin/windows/base/release.htm).
* Run the `.exe` file that was just downloaded
* Go to the [RStudio download page](https://www.rstudio.com/products/rstudio/download/#download)
* Under *Installers* select **RStudio x.yy.zzz - Windows Vista/7/8/10** (where x, y, and z represent version numbers)
* Double click the file to install it
* Once it's installed, open RStudio to make sure it works and you don't get any error messages.

**macOS**
- If you already have R and RStudio installed
* Open RStudio, and click on "Help" > "Check for updates". If a new version is available, quit RStudio, and download the latest version for RStudio.
* To check the version of R you are using, start RStudio and the first thing that appears on the terminal indicates the version of R you are running. Alternatively, you can type `sessionInfo()`, which will also display which version of R you are running. Go on the [CRAN website](https://cran.r-project.org/bin/macosx/) and check whether a more recent version is available. If so, please download and install it.

- If you don't have R and RStudio installed
* Download R from the [CRAN website](https://cran.r-project.org/bin/macosx/).
* Select the `.pkg` file for the latest R version
* Double-click on the downloaded file to install R
* It is also a good idea to install [XQuartz](https://www.xquartz.org/) (needed by some packages)
* Go to the [RStudio download page](https://www.rstudio.com/products/rstudio/download/#download)
* Under *Installers* select **RStudio x.yy.zzz - Mac OS X 10.6+ (64-bit)** (where x, y, and z represent version numbers)
* Double-click the file to install RStudio
* Once it's installed, open RStudio to make sure it works and you don't get any error messages.

**Linux**
* Follow the instructions for your distribution from [CRAN](https://cloud.r-project.org/bin/linux), they provide information to get the most recent version of R for common distributions. For most distributions, you could use your package manager (e.g., for Debian/Ubuntu run `sudo apt-get install r-base`, and for Fedora `sudo yum install R`), but we don't recommend this approach as the versions provided by this are usually out of date. In any case, make sure you have at least R 3.5.1.
* Go to the [RStudio download page](https://www.rstudio.com/products/rstudio/download/#download)
* Under *Installers* select the version that matches your distribution, and install it with your preferred method (e.g., with Debian/Ubuntu `sudo dpkg -i rstudio-x.yy.zzz-amd64.deb` at the terminal).
* Once it's installed, open RStudio to make sure it works and you don't get any
   error messages.



Once you have R and R Studio installed, open R Studio 
1.  Go to File>New Project> Version Control >Git
2.  Enter the Repository URL [https://github.com/DCS-training/DH-RSESummerSchool2024/day%1](https://github.com/DCS-training/DH-RSESummerSchool2024/day%1)
3.  Select the Name for the directory project and where to save it
4.  Press Create Project 


#### Installation of Needed Packages 
The packages we are going to need for this workshop are the below
for Part 1: 
`install.packages("tidyverse")`

`install.packages("palmerpenguins")`

for Part 2:
`install.packages("tmap")`

`install.packages("sf")`

`install.packages("RColorBrewer")`

for Part 3:
`install.packages("tidytext")`

`install.packages("janeaustenr")`

`install.packages("magick") `

`install.packages("devtools")` 

Please make sure to run the above packages ahead of time 

### Custom data visualisation with D3

D3 is a popular JavaScript library for data visualization that lets you create fully custom visualizations. Observable is an online platform that lets you easily get started with D3, even if you have no prior experience with JavaScript. Observable notebooks let you upload and use data and are great for prototyping web-based data visualizations. This course will provide a basic introduction to the D3 library and the Observable platform, allowing you to build on these skills independently afterwards.

No Pre-setting is needed besides creating an account in the Observable platform [https://observablehq.com/](https://observablehq.com/)  




## Licence of the material
All the material collected here is covered by a CC-BY-NC 4.0 License
