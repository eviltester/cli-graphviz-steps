# cli-graphviz-steps

generate animated graphviz from the command line

```
npm install
```

Pre-requisites:

- Have an http server running on `localhost:8080`
- Have [ffmpeg installed](https://ffmpeg.org/)
- Have [Chrome Browser](https://www.google.com/intl/en_uk/chrome/) installed


Running an Http Server easily with python.

e.g.

```
python3 -m http.server
```

Run the app:

```
node index.js example-anim.dot
```

- the `example-anim.dot` will be injected in the `create-anim-file.html`
- `create-anim-file.html` will be opened in Chrome
- an output folder will be created
- the animation will be saved into the output folder as a series of `.png` files
- `ffmpeg` will be used to convert all the `.png` files into an `.mp4` file in the output folder
