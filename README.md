# thirdweb-art-engine

## Setup Instructions

### Prerequisites
- [Git](https://git-scm.com/)
- [Node Version Manager (nvm)](https://github.com/nvm-sh/nvm) for Mac/Linux  
- [nvm-windows](https://github.com/coreybutler/nvm-windows) for Windows

---

### 1. Clone the Repository

```sh
git clone https://github.com/0xteksage/thirdweb-art-engine.git
cd thirdweb-art-engine
```

---

### 2. Install Node.js (Recommended: v20 LTS)

#### **Windows**
1. Download and install [nvm-windows](https://github.com/coreybutler/nvm-windows/releases).
2. Open Command Prompt and run:
   ```sh
   nvm install 20
   nvm use 20
   node -v   # Should show v20.x.x
   ```

#### **Mac/Linux**
1. Install nvm:
   ```sh
   curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
   ```
2. Restart your terminal, then run:
   ```sh
   nvm install 20
   nvm use 20
   node -v   # Should show v20.x.x
   ```

---

### 3. Install Dependencies

```sh
npm install
```

---

...

### 4. Run the Art Engine

#### EVM-Compatible Art Generation
To generate art for EVM-compatible chains (like Ethereum, Polygon, etc.), use:
```sh
npm run generate
```

#### Sei Chain
- **AR Format:**
  ```sh
  npm run seiBuild:ar
  ```
- **NS Format:**
  ```sh
  npm run seiBuild:ns
  ```

#### Solana Chain
- **AR Format:**
  ```sh
  npm run solBuild:ar
  ```
- **NS Format:**
  ```sh
  npm run solBuild:ns
  ```

---

### Troubleshooting

- If you encounter errors with the `canvas` package, make sure you are using Node.js v20 LTS.
- On Windows, you may need to install additional build tools:
  ```sh
  npm install --global windows-build-tools
  ```
- For more help, see the [canvas installation guide](https://www.npmjs.com/package/canvas#compiling)