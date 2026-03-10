# La Paradoja Colombiana Project 🌟

[![license](https://img.shields.io/badge/license-MIT-brightgreen)](./LICENSE) [![notebook](https://img.shields.io/badge/Jupyter-Notebook-orange)](world_happiness_report_imgs.ipynb) [![open in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/your-username/La-Paradoja-Colombiana/blob/main/world_happiness_report_imgs.ipynb)

La Paradoja Colombiana is a web application and data-analysis project that presents a visually appealing, interactive narrative exploring the paradox of happiness in Colombia despite economic challenges and social inequality. The front-end narrative is driven by `index.html` and styles, while `world_happiness_report_imgs.ipynb` contains the analysis and visualizations based on the World Happiness Report.

Demo: (Add a live demo link here if available)

Table of Contents
- Features
- Tech Stack
- Installation
- Run Locally
- Usage / Examples
- Project Structure
- Screenshots
- Environment Variables
- Contributing
- Tests
- License
- Contact
- Acknowledgements


Badges

Place badges near the top (license, notebook/colab, build, coverage). Example (already included above):

[![license](https://img.shields.io/badge/license-MIT-brightgreen)](./LICENSE) [![notebook](https://img.shields.io/badge/Jupyter-Notebook-orange)](world_happiness_report_imgs.ipynb) [![open in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/your-username/La-Paradoja-Colombiana/blob/main/world_happiness_report_imgs.ipynb)


## 🚀 Features
- Interactive narrative divided into sections or "story blocks" 📚
- Responsive design ensuring adaptability to different screen sizes and devices 📱
- Integration of data analysis and visualization from the World Happiness Report 📊
- Google Fonts for improved typography 📄
- Potential interactive elements (scroll indicators, responsive images) 🖼️

Notes: Consider adding progressive enhancements (lazy loading images, accessible ARIA attributes) and more interactive charts (D3.js or Plotly) for richer data exploration.


## 🛠️ Tech Stack
- HTML5 & CSS3
- Google Fonts API
- Python 3.8+ for data analysis
- Jupyter Notebook / Google Colab
- pandas, numpy, matplotlib (add seaborn or plotly as needed)

Tip: Add a requirements.txt with pinned versions (e.g., pandas==1.5.3) for reproducibility.


## 📦 Installation
A step-by-step guide to get the project running locally.

1) Clone the repo
```bash
git clone https://github.com/your-username/La-Paradoja-Colombiana.git
cd La-Paradoja-Colombiana
```

2) (Optional) Create a virtual environment and activate it
```bash
python3 -m venv venv
# Linux / macOS
source venv/bin/activate
# Windows (PowerShell)
.\venv\Scripts\Activate.ps1
```

3) Install Python dependencies (if you plan to run notebooks)
```bash
pip install -r requirements.txt
```

If you don't have a requirements.txt yet, at minimum install:
```bash
pip install jupyter pandas numpy matplotlib
```

4) Open the notebook or the web app (see Run Locally)


Run Locally

To view the front-end narrative:
- Option A: Open `index.html` directly in your browser (double-click or right-click -> Open With).
- Option B (recommended for relative assets): serve via a simple HTTP server:

```bash
# Python 3
python -m http.server 8000
# Then visit http://localhost:8000 in your browser
```

To run the analysis notebook:
- Start Jupyter locally:
```bash
jupyter notebook world_happiness_report_imgs.ipynb
```
- Or open the notebook in Google Colab (badge above links to an example). If you add large data files, prefer Colab for easier execution.


## 💻 Usage
- View the interactive narrative: open `index.html` or serve the directory as described in Run Locally.

- Notebook usage: open `world_happiness_report_imgs.ipynb` and run cells. Key example to load data (in notebook):

```python
import pandas as pd
df = pd.read_csv('data/happiness_report_data.csv')
df.head()
```

- To reproduce figures, run all notebook cells. If using Google Colab, upload the `data/` folder or mount Google Drive.


## 📂 Project Structure
```
La-Paradoja-Colombiana/
│
├── index.html
├── style.css
├── world_happiness_report_imgs.ipynb
├── WHR25_Data_Figure_2.1.xlsx
├── images/
│   ├── image1.jpg
│   ├── image2.jpg
│   └── ...
├── data/
│   ├── happiness_report_data.csv
│   └── ...
├── notebooks/
│   ├── world_happiness_report_imgs.ipynb
│   └── ...
├── README.md
└── LICENSE
```

Add these recommended files if missing:
- `requirements.txt` (for notebook reproducibility)
- `CONTRIBUTING.md` (contribution workflow)
- `CODE_OF_CONDUCT.md`
- `.gitignore`


## 📸 Screenshots



![Home screen screenshot](https://github.com/SantiagoQP31/proyecto-introduccion-cdos/imgs/ss.png)





Environment Variables

This project does not require secret environment variables for the front-end or the notebooks by default. If you integrate APIs later (e.g., map or chart APIs), document any required keys here and how to set them (e.g., .env file or GitHub Actions secrets).


## 🤝 Contributing
Thank you for your interest in contributing! To make collaboration smooth, please follow these steps:

1. Fork the repository.
2. Create a feature branch: `git checkout -b feat/short-description`.
3. Commit your changes with descriptive messages.
4. Push to your fork and open a Pull Request to `main`.

Guidelines:
- Keep changes focused and small.
- Include screenshots or notebook outputs for visual changes.
- If adding Python dependencies, update `requirements.txt`.

Optional: Add `CONTRIBUTING.md` and `CODE_OF_CONDUCT.md` to the repository with more details.


Running Tests

There are no automated tests included at the moment. Consider adding unit tests for any Python data-processing modules (pytest) and basic accessibility or HTML tests for the front-end.


## 📝 License
This project is licensed under the MIT License — see the LICENSE file for details.

[View LICENSE](./LICENSE)


## 📬 Contact
For questions or suggestions, open an issue in GitHub or contact the maintainers:

- Maintainer: Your Name (replace with actual name)
- Email: your-email@example.com (replace with real contact)
- Repository: https://github.com/your-username/La-Paradoja-Colombiana

If you prefer, add a CONTRIBUTORS.md with more contact details and responsibilities.


## 💖 Thanks & Acknowledgements
A heartfelt thanks to all contributors and supporters of the La Paradoja Colombiana project. Your contributions and feedback are invaluable.

This README was initially generated with help from [readme.ai](https://readme-generator-phi.vercel.app/). Please add any third-party libraries, data sources, or references used in the project here (e.g., World Happiness Report dataset citation).


Appendix / Next Steps

Suggestions for future improvements:
- Add a requirements.txt and CI checks (e.g., GitHub Actions to run notebooks or linting).
- Add tests for data processing.
- Add a live demo deployment (GitHub Pages or Netlify) and include the link near the top.
- Add accessibility & performance optimizations for the front-end.
