# Jazzicon SVG Generator

A simple Jazzicon SVG Generator for Ethereum addresses.

## Installation

```
npm i @raugfer/jazzicon
```

## Usage

```typescript jsx
// sample code for react component
import Jazzicon from '@raugfer/jazzicon';

export default function JazziconImage({ address }: { address: string }) {
  const imageUrl = 'data:image/svg+xml;base64,' + btoa(Jazzicon(address));
  return (
    <img src={imageUrl} alt="Jazzicon" />
  );
}
```
