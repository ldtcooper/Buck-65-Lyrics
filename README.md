# README
Ever since coming across Matt Daniel's Rapper Vocabulary Chart, I've been interested in how one of my favorite rappers -- Buck 65 -- would place on there, and this is my attempt at finding that out.

## Instructions
Everything that you need to reproduce these results is included in the file. Due to copyright concerns, I haven't included any of the lyrics data in my repository, but `buck65.ipynb` has all of the steps to gather it.
First up will be setting up the conda environment. Running `setup.sh` should suffice to install all dependencies and start up a conda enviornment, but if it doesn't try running the commands:
```sh
$ conda env create --file environment.yml #creates the enviornment from the YAML file
$ conda activate buck65 # activates the enviornment
```

After that, you will need to get Genius API access. Follow the instructions [here](https://docs.genius.com/) to get that set up. Once you have your keys, create a copy of `secrets.json.template` called `secrets.json` and copy in your Genius API keys, or at least your client access token under the field `CLIENT_ACCESS_TOKEN`. With that done, you should be able to reproduce my results.

## Sources
- https://rareloot.medium.com/how-to-download-an-artists-lyrics-from-genius-com-using-python-984d298951c6