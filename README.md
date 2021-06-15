# Personal Score Partner API
Repository for Personal Score Partner API documentation.

## Local Development
You can build and export the documentation locally outside Apiary with a few simple steps. All you need is working Node.js environment on your machine.

1. Clone this repository
```bash
git clone git@github.com:zonkyio/zscore-partner-api.git
cd zscore-partner-api
```

2. Install project dependencies
```bash
npm install
```

3. Run development server
```bash
npm run dev
```
Server will start on `http://localhost:3000` and will listen for changes in `apiary.apib` file.

4. Export documentation
```bash
npm run build
```

## Local build with docker
1. Pull image 
```bash
docker pull apiaryio/client
```

2. Export documentation
```bash
docker run -v $(pwd):/tmp apiaryio/client preview --output=/tmp/result.html --path=/tmp/apiary.apib
```

The documentation will be exported to a single `result.html` file.
## Further Reading / Useful Links

- [API Blueprint](https://apiblueprint.org)
