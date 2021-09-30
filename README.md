# Quansight-Labs-Presentation

The slides and content for the internship talk at [Quansight Labs](https://labs.quansight.org) on re-engineering CI/CD pipelines for [Scipy](https://github.com/scipy/scipy).

## Setup

To setup the slides on your local machine, follow these steps:

1. Install  [hugo](https://gohugo.io/getting-started/installing/)
2. For development:

	```sh
	hugo server -D
	```

3. In  `config.toml`  set  `baseURL`  to be the baseURL of your hosted website.
4. To build and serve it using Docker, push the following command:

	```sh
	docker run --rm -it \
	  -v $(pwd):/src \
	  -p 1313:1313 \
	  klakegg/hugo:0.83.1 \
	  server
	```

## Acknowledgements

The slide format is inspired from [Anirudh Dagar's Quansight Labs Internship talk](https://github.com/AnirudhDagar/qs-intern-talk) and [Thomas J. Fan's Hugo+Reveal Slide template](https://github.com/thomasjpfan/slides-template-hugo).
