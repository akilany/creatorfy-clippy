# creatorfy-clippy

Using Clippy and its friends in your React Application it has never been easier!

## Instalation

### Using yarn

```bash
yarn add creatorfy-clippy
```

### Using npm

```bash
npm install --save creatorfy-clippy
```

## Usage

```jsx
import { useClippy, ClippyProvider } from "creatorfy-clippy";

const MyComponent = () => {
  const { clippy } = useClippy();

  return <Button onClick={() => clippy.play("Wave")}>Hello Clippy!</Button>;
};

const App = () => (
  <ClippyProvider>
    <MyComponent />
  </ClippyProvider>
);
```

### Changing the Agent

```jsx
import { AGENTS } from "creatorfy-clippy";

const App = () => (
  <ClippyProvider agentName={AGENTS.MERLIN}>
    <MyComponent />
  </ClippyProvider>
);
```

## API and Special thanks

This package only exposes the brilliant job done in
[clippyjs](https://github.com/pi0/clippyjs) project, which you can find all details you'll need.
