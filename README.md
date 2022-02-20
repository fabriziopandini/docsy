# Docsy Example

[Docsy][] is a [Hugo theme][] for technical documentation sites, providing easy
site navigation, structure, and more. 

In this project, I'm playing around hugo and docsy template for adoption on Cluster API.

## TODO

There is still a long way to do...

### Look and feel

- [ ] make sure featured-background on "home", "about" and "community" scales properly on xl screens
- [ ] on small devices convert navbar menu to drop list
- [ ] prevent .td-sidebar to go under the logo when scrolling down
- [ ] 404
- [ ] figure out how to share the same featured-background on "home", "about" and "community" without duplicating it
- [ ] give credits for the featured-background to https://unsplash.com/photos/KABfjuSOx74 

### Missing features

- [ ] Link checker
- [ ] Embed github (iframe??)

### Content

- [ ] complete work on "home", "about" and "community"
  - [ ] thing to key messages in home (multi cloud, like Kubernetes, manage etc, might be an example)
  - [ ] ensure "about" and "community" can have look and feel like home page at top and content below
- [ ] validate the idea of three main doc area (user, provider, developer)
  - [ ] map existing docs on those area
  - [ ] validate if to show them in navbar (and eventually drop documentation)

### Miscellaneus

- [ ] Investigate if to preserve the sub module to get theme updates or drop
- [ ] Check how to move everything to sub folder (except build and netlify)
- [ ] Check integration with netlify

## Running a container locally

You can run docsy-example inside a [Docker](https://docs.docker.com/)
container, the container runs with a volume bound to the `docsy-example`
folder. This approach doesn't require you to install any dependencies other
than [Docker Desktop](https://www.docker.com/products/docker-desktop) on
Windows and Mac, and [Docker Compose](https://docs.docker.com/compose/install/)
on Linux.

1. Build the docker image 

   ```bash
   docker-compose build
   ```

1. Run the built image

   ```bash
   docker-compose up
   ```

   > NOTE: You can run both commands at once with `docker-compose up --build`.

1. Verify that the service is working. 

   Open your web browser and type `http://localhost:1313` in your navigation bar,
   This opens a local instance of the docsy-example homepage. You can now make
   changes to the docsy example and those changes will immediately show up in your
   browser after you save.

### Cleanup

To stop Docker Compose, on your terminal window, press **Ctrl + C**. 

To remove the produced images run:

```console
docker-compose rm
```
For more information see the [Docker Compose
documentation](https://docs.docker.com/compose/gettingstarted/).

## Troubleshooting

As you run the website locally, you may run into the following error:

```
➜ hugo server

INFO 2021/01/21 21:07:55 Using config file: 
Building sites … INFO 2021/01/21 21:07:55 syncing static files to /
Built in 288 ms
Error: Error building site: TOCSS: failed to transform "scss/main.scss" (text/x-scss): resource "scss/scss/main.scss_9fadf33d895a46083cdd64396b57ef68" not found in file cache
```

This error occurs if you have not installed the extended version of Hugo.
See our [user guide](https://www.docsy.dev/docs/getting-started/) for instructions on how to install Hugo.

[alternate dashboard]: https://app.netlify.com/sites/goldydocs/deploys
[deploys]: https://app.netlify.com/sites/docsy-example/deploys
[Docsy user guide]: https://docsy.dev/docs
[Docsy]: https://github.com/google/docsy
[example.docsy.dev]: https://example.docsy.dev
[Hugo theme]: https://www.mikedane.com/static-site-generators/hugo/installing-using-themes/
[Netlify]: https://netlify.com
