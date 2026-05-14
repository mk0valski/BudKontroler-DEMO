# BudKontroler-DEMO
BudKontroler is a Python App for DXF drawings quality control. It checks the layer schema, geometry types of entities, and topology. The user receives a text report as a result, which can be easily imported into CAD software.

# How it works
App based on ezdxf and PySimpleGui libraries. The user inputs a DXF file and sets a buffer size of a minimum length between vertex neighbours. The analysis of the sketch is divided into:
  1. Renaming layers to the company schema.
  2. Deleting points that are useless in our case.
  3. Checking the entity type in text and polyline layers.
  4. Counting vertex duplicates to find topological errors.
  5. Searching for vertices closer than the value input by the user.
  6. Saving an error message in a multiline label and text file.

# Visualization
https://github.com/user-attachments/assets/88ca260e-8694-49e2-ba7b-5f554896f77c
