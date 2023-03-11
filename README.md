
<p align="center" style="font-weight: bold; font-size: 1.5em">@bit-about/context</p>
<p align="center">
<a href="https://www.npmjs.com/package/@bit-about/context"><img alt="" src="https://img.shields.io/npm/v/@bit-about/context.svg" /></a>
<a href="https://bundlephobia.com/package/@bit-about/context"><img alt="Bundle size" src="https://img.shields.io/bundlephobia/minzip/@bit-about/context?label=size" /></a>
</p>

## Install

```bash
npm i @bit-about/context
```

## Description

Aimed at delivering context-related utils for @bit-about libraries. 

- 100% **Idiomatic React** and 100% Typescript
- Tiny & Efficient
- Does not trigger unnecessary renderings
- as always, **Just works** ™

## Usage

```tsx
import { createContext, useContextSelector } from '@bit-about/context'

interface State {
  alice: number;
  bob: number;
}

const defaultValue: State = {
  alice: 1,
  bob: 2
}

const Context = createContext<State>(defaultValue)

const App = () => (
  <Context.Provider value={defaultValue}>
    <Component />
  </Context.Provider>
)

const Component = () => {
  const bob = useContextSelector(Context, (state) => state.bob)

  return bob // returns "2"
}
```



## Partners  
<a href="https://www.wayfdigital.com/"><img alt="wayfdigital.com" width="100" height="100" src="https://user-images.githubusercontent.com/1496580/161037415-0503f763-a60b-4d40-af9f-95d1304fa486.png"/></a>

## Credits
- [use-context-selector](https://github.com/dai-shi/use-context-selector) & [FluentUI](https://github.com/microsoft/fluentui) - fancy re-render avoiding tricks and code main inspiration

## License
MIT © [Maciej Olejnik 🇵🇱](https://github.com/macoley)

## Support me 

<a href="https://github.com/sponsors/macoley"><img alt="Support me!" src="https://img.shields.io/badge/github.com-Support%20me!-green"/></a>

If you use my library and you like it...<br />
it would be nice if you put the name `BitAbout` in the work experience section of your resume.<br />
Thanks 🙇🏻! 


---
<p align="center">🇺🇦 Slava Ukraini</p>
