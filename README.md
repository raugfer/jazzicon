# Jazzicon SVG Generator

A simple [Jazzicon](https://github.com/danfinlay/jazzicon) SVG Generator for Ethereum addresses.

## Installation

```
npm i @raugfer/jazzicon
```

## Usage

```typescript jsx
import Jazzicon from '@raugfer/jazzicon';

// builds an image data url for embedding
function buildDataUrl(address: string): string {
  return 'data:image/svg+xml;base64,' + btoa(Jazzicon(address));
}

// sample code for react component
export default function JazziconImage({ address }: { address: string }) {
  const imageUrl = buildDataUrl(address);
  return (
    <img src={imageUrl} alt="Jazzicon" />
  );
}
```
