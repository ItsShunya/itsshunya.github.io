# shunya.is-a.dev

My personal website!

# Development Environment

Install Hugo (the following command also installs Go):  
```
$ sudo apt install hugo
```

Clone the repository with its submodules.
```
git clone git@github.com:ItsShunya/shunya.is-a.dev.git --recursive blog
```

# Run it locally

To launch the development site:  
```
hugo server --minify -D -E -F
```

# Deployment

Currently, the deployment is performed automatically thanks to Github Actions! On every push to `main` branch, the CI will update the Github Page with the latest changes.