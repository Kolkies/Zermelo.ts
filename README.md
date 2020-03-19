# Zermelo.ts
> The package for using the zermelo api

## Installation

```bash
yarn install zermelo.ts # Or npm install zermelo.ts
```

## Example

```js
const { Zermelo } = require("zermelo.ts");
const asyncFunction = async () => {
  const accessToken = await Zermelo.getAccessToken("schoolnaam", "koppel_code");
  const ZermeloAPI = Zermelo.getAPI("schoolnaam", accessToken);
  const userInfo = await ZermeloAPI.users.get();
  console.log(userInfo);
};

asyncFunction();
```

## Licensing
The code in this project is licensed under MIT license.
