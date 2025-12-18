# **keys.** | Secure API Key Generator

**keys.** is a privacy-focused, client-side API key generator built with [Astro](https://astro.build). It generates cryptographically secure keys (UUIDs, Hex tokens, Base64 strings) directly in your browser using the Web Crypto API.

## Key Features

- 🔒 **100% Client-Side**: No backend, no analytical tracking, and no data transmission. Keys are generated locally in your browser memory.
- 🛡️ **Cryptographically Secure**: Uses `window.crypto.getRandomValues` for high-entropy generation.
- ⚡ **Zero Latency**: Instant generation with no network requests.
- 👁️ **Visual Privacy**: Keys are masked on-screen (`••••`) to prevent shoulder surfing. Click "Copy" to retrieve the actual key.
- 🎨 **Professional SaaS Design**: Clean, compact, and responsive interface modeled after high-end developer tools.

## Tech Stack

- **Framework**: [Astro](https://astro.build) (Static Site Generation)
- **Language**: TypeScript / JavaScript
- **Styling**: Vanilla CSS (Scoped & Global variables)
- **Font**: [Inter](https://fonts.google.com/specimen/Inter)

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm

### Installation

1.  Clone the repository:

    ```bash
    git clone https://github.com/your-username/api-key-generator.git
    cd api-key-generator
    ```

2.  Install dependencies:

    ```bash
    npm install
    ```

3.  Run the development server:
    ```bash
    npm run dev
    ```
    Open `http://localhost:4321` in your browser.

### Building for Production

To create a production build (static HTML/CSS/JS):

```bash
npm run build
```

You can preview the build locally:

```bash
npm run preview
```

## Security Note

This application relies on the browser's `crypto` API. While suitable for generating API keys, session tokens, and IDs, please ensure your local machine is secure. Since no data leaves your browser, the security of the generated keys depends entirely on your local environment.

## License

MIT
