# RICON 2026 Certificate Generator Web App

A lightweight, zero-backend, client-side certificate generator and live preview portal designed for the **RICON 2026** conference (Department of Radiodiagnosis, IMS BHU & Varanasi Chapter of IRIA).

Built specifically for **Vercel Free Tier** with zero server costs, zero cold starts, and instantaneous browser-side PDF generation using `pdf-lib`.

---

## Features

- **6 Certificate Categories**:
  1. **Faculty**: Centered, bolded name above the signature line.
  2. **Organizing Committee (OC)**: Dedicated OC certificate template.
  3. **Delegate**: Centered name above line and institute name below line.
  4. **Oral Presenter**: Name, institute, and presentation title.
  5. **E-Poster Presenter**: Name, institute, and presentation title.
  6. **Case Report Presenter**: Name, institute, and presentation title.
- **Dynamic Dialog / Form**: Inputs automatically adjust based on the selected certificate type.
- **Auto-Formatting & Text Wrapping**: Automatically calculates center alignment and wraps multi-line presentation titles seamlessly.
- **Standardized Naming Convention**: Generates files named `firstname_secondname_certificatetype.pdf` (e.g., `Anuradha_Singh_oral_presentation.pdf`).
- **Live In-Browser Preview**: Users can preview their generated certificate in high resolution before saving.

---

## Local Testing

You can test this locally in 5 seconds using Python or Node:

### Using Python:
```bash
cd ricon-cert-portal
python3 -m http.server 3000
```
Then open: [http://localhost:3000](http://localhost:3000)

### Using Node / npx:
```bash
cd ricon-cert-portal
npx serve .
```

---

## Deploying to Vercel (Free Tier)

### Method 1: Via Vercel CLI (Fastest)
1. In your terminal, navigate to the portal folder:
   ```bash
   cd "ricon-cert-portal"
   ```
2. Run:
   ```bash
   npx vercel
   ```
3. Follow the 3 prompts (choose default settings). Your live site will be deployed in under 30 seconds!

### Method 2: Via GitHub + Vercel Dashboard
1. Push the `ricon-cert-portal` folder or its repository to your GitHub account.
2. Go to [vercel.com/new](https://vercel.com/new).
3. Import the repository and click **Deploy**.
4. Since this is a static site with no complex build steps required, Vercel will deploy it instantly for free.
