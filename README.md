# eslint-config-deriv-beta
This package provides Deriv's .eslintrc as an extensible shared config.

# installation
 For **deriv-com:**
 

 1. remove the below packages from package.json:
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

# Usage
inside `.eslinrc` remove `plugins` , `rules` , `env`, `parser` , and `settings` and then change "extends" like this:

    "extends": ["eslint:recommended", "deriv-beta"]
and to test if it's working run the bellow command: 

    npm run eslint
