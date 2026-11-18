# Nate Puangpanbut: Data Science Portfolio

**Live site → [suraporn.github.io/ds](https://suraporn.github.io/ds/)**

This is my personal portfolio as a Senior Data Scientist. It covers my experience, my résumé, and write-ups of projects in forecasting, machine learning, MLOps, deep learning and statistics.

## What's inside

| Page | What it covers |
|---|---|
| **Home** | Summary, highlights and selected projects |
| **Projects** | 13 write-ups, each with code and figures |
| **Resume** | Experience, education, skills and certifications, plus a PDF download |
| **Contact** | A message form and links |

### Project write-ups

| Area | Projects |
|---|---|
| MLOps & deployment | Operationalizing ML models with GCP Vertex AI · Deploying ML models with Docker, Flask and FastAPI |
| Machine learning | Tuning classifiers on imbalanced data · Precision-Recall vs ROC curves · GridSearchCV vs RandomizedSearchCV · Airbnb listing rating prediction |
| Statistics | EPL ranking with Bayesian inference |
| Deep learning & vision | My GAN Wife (GANs) · Neural networks and their applications · Seam carving (content-aware resizing) |
| Data | Common mistakes in SQL |

## Built with

The site is plain HTML and CSS, with no framework and no build step. It's hosted free on GitHub Pages.

- **Responsive layout:** a single stylesheet (`style.css`) styles every page, using Inter and JetBrains Mono.
- **Images:** sized for the web. Photos and screenshots are capped at 1,600 px, and animations are kept as looping GIFs.
- **No tracking:** the only external resource is Google Fonts.

## Structure

```
home.html           Home page
index.html          Redirects to home.html
projects.html       Project index
resume.html         Résumé
contact.html        Contact form
post/               One page per project write-up
images/             Profile photo, project thumbnails, figures, certificates
files/resume.pdf    Downloadable résumé
style.css           Shared styles
```

## Run it locally

```
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Updating

- **Add a project:** copy any file in `post/` as a template. Add its thumbnail to `images/projects/<slug>.jpg`, then add a card to `projects.html`. To feature it on the home page, add the card to `home.html` too.
- **Update the résumé:** replace `files/resume.pdf` and edit `resume.html`. Bump the `?v=` number on the résumé links so browsers fetch the new PDF.
- **Style changes:** after editing `style.css`, bump the `?v=` number in the stylesheet links, so visitors' browsers load the new version.

## Contact

nate.puangpanbut@gmail.com · [LinkedIn](https://www.linkedin.com/in/suraporn/) · [GitHub](https://github.com/Suraporn) · [Medium](https://medium.com/@suraporn83)
