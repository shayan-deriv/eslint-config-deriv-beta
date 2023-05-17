# eslint-config-deriv-beta
This package provides Deriv's .eslintrc as an extensible shared config.

# installation
 For **deriv-com:**
 

 1. remove the below packages from package.json in root and also each packages:
	 - `"eslint-import-resolver-node": "^0.3.6"`
	 - `"@typescript-eslint/eslint-plugin": "^5.9.0"`
	 - `"@typescript-eslint/parser": "^5.9.0"`
	 - `"eslint": "^7.32.0"`
	 - `"eslint-loader": "^4.0.2"`
	 - `"eslint-plugin-deprecation": "^1.3.2"`
	 - `"eslint-plugin-import": "^2.25.4"`
	 - `"eslint-plugin-jest": "^26.1.4"`
	 - `"eslint-plugin-react": "^7.28.0"`
	 - `"eslint-plugin-react-hooks": "^4.5.0"`
	 - `"eslint-webpack-plugin": "^3.1.1"`
	 
 2.  Install the latest version:

    npm i eslint-config-deriv-beta

 For **deriv-app:**
 1. remove the below packages from package.json:
	  - `"@typescript-eslint/eslint-plugin": "^5.8.0"`
	  - `"@typescript-eslint/parser": "^5.8.0"`
	  - `"eslint": "^7.18.0"`
	  - `"eslint-config-airbnb-base": "^14.2.1"`
	  - `"eslint-config-binary": "^1.0.2"`
	  - `"eslint-config-prettier": "^7.2.0"`
	  - `"eslint-formatter-pretty": "^4.0.0"`
	  - `"eslint-import-resolver-typescript": "^2.7.1"`
	  - `"eslint-import-resolver-webpack": "^0.13.0"`
	  - `"eslint-plugin-import": "^2.23.4"`
	  - `"eslint-plugin-jest-dom": "^3.8.1"`
	  - `"eslint-plugin-prettier": "^3.3.1"`
	  - `"eslint-plugin-react": "^7.22.0"`
	  - `"eslint-plugin-react-hooks": "^4.2.0"`
	  - `"eslint-plugin-testing-library": "^4.2.0"`

 2.  add the below to the **devDependencies** of the root `package.json`:

	   "eslint-config-deriv-beta": "^1.0.2"

 3.  run `npm run i` and then `npm run bootstrap`

# Usage
For **deriv-com:**
inside `.eslinrc` remove `plugins` , `rules` , `env`, `parser` , and `settings` and then change "extends" like this:

    "extends": ["eslint:recommended", "deriv-beta"]
and to test if it's working run the bellow command: 

    npm run eslint

For **deriv-app:**
inside `.eslinrc` remove everything except `overrides` and add this at the top :

    "extends": ["deriv-beta"]
and to test if it's working run the bellow command: 

    npm run test:eslint-all
