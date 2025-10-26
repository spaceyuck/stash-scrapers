Scrapers created or modified by me. To use you need to have [stashapp/stash](https://github.com/stashapp/stash) application.

Source index: [`https://spaceyuck.github.io/stash-scrapers/main/index.yml`](https://spaceyuck.github.io/stash-scrapers/main/index.yml)

## Install 

1. To add a new source go to **Settings** > **Metadata Providers** page.
1. Under Available Scrapers click **Add Source**.
1. Add the following details:
    - Name: `spaceyuc`
    - Source URL: `https://spaceyuck.github.io/stash-scrapers/main/index.yml`
    - Local path: `spaceyuc`
1. Click Confirm.
1. Under Available Scrapers select **spaceyuc** package to expand it and see all available scrapers.
1. Click the checkmark next to relevant scraper and click **Install**.

## Contributing

Pull requests are welcome.

### Repository structure

- Each yaml scraper should be under proper folder based on the website name (`./scrapers/<website>`). 
- Multiple scrapers can be under the same `<website>` folder.
- Scrapers with only yaml files should be in the root folder under the `<website>`. 
- Scrapers with files that have dependancies should have its own folder under the `<website>` root.

### Validation

The scrapers in this repository can be validated against a schema and checked for common errors.

First, install the validator's dependencies - inside the [`/validator`](./validator) folder, run: `yarn`.

Then, to run the validator, use `node validate.js` in the root of the repository.
Specific scrapers can be checked using: `node validate.js scrapers/folder/example.yml scrapers/folder2/example2.yml`

## Attributions

From [https://github.com/stashapp/CommunityScrapers](https://github.com/stashapp/CommunityScrapers) under AGPL-3.0:

- `./validate.js`
- `./build-site.sh`
- `./validator/*`
- `./.github/workflows/validate.yml`