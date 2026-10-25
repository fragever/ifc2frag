# ifc2frag

A small web app that converts IFC building models into That Open Company's
[Fragments 2.0](https://github.com/ThatOpen/engine_fragment) `.frag` format, the
format [FragmentsUnreal](https://github.com/fragever/FragmentsUnreal) loads into
Unreal Engine.

You can also open an existing `.frag` file to check it before you bring it into
Unreal.

**Don't want to install anything?** The hosted version runs at
[fragmentsunreal.dev/viewer](https://www.fragmentsunreal.dev/viewer/).

Either way, the conversion runs in your browser, so your model isn't uploaded
anywhere. Running it locally still fetches the `web-ifc` engine and the
Fragments worker from public CDNs, so it needs an internet connection.

---

## 🚀 Getting Started

### Requirements

- Node.js 20.19+ or 22.12+ (required by Vite 7)
- npm

### Install and run

```bash
git clone https://github.com/fragever/ifc2frag.git
cd ifc2frag
npm install
npm run dev
```

Then open [http://localhost:5173](http://localhost:5173) in your browser.

---

## 🔄 Converting a model

1. Click **Load IFC** and pick your `.ifc` file. Large models can take a while;
   the model shows in the viewer when the conversion is done.
2. Click **Download**, name the file, and save it as a `.frag`.
3. Load that `.frag` in Unreal with FragmentsUnreal. The
   [getting started guide](https://www.fragmentsunreal.dev/docs/getting-started)
   covers the Unreal side.

**Load Frag** opens an existing `.frag` file in the viewer, and **Clear** empties
the scene.

---

## 🛠 Powered by

* [`@thatopen/components`](https://www.npmjs.com/package/@thatopen/components)
* [`@thatopen/fragments`](https://www.npmjs.com/package/@thatopen/fragments)
* [`@thatopen/ui`](https://www.npmjs.com/package/@thatopen/ui)
* [`web-ifc`](https://github.com/ThatOpen/engine_web-ifc)

---

## 🛡 License

[MIT](./LICENSE)
