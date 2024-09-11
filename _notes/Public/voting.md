---
title: Voting
feed: show
date: 01-01-2021
---

En [[Machine Learning]] es una técnica de ensamble en la que varios [[modelo|modelos]] (a menudo de diferentes tipos) hacen predicciones independientes y la respuesta final se decide mediante un "voto" entre ellos. Hay dos formas principales: **"hard voting"** donde la clase con más votos gana, y **"soft voting"** donde se promedian las probabilidades de predicción de cada clase y la clase con el promedio más alto gana.

>[!done]+ Analogia
>Imagina que estás tratando de decidir qué película ver y consultas a tres amigos. Uno prefiere **acción, otro comedia, y otro drama**. En *"hard voting"*, si dos sugieren comedia, esa es la elegida. En *"soft voting"*, consideras cuánto les gusta cada género y eliges basado en el promedio de sus preferencias. 

>[!note]+ Es igual que [[bagging]]?
>Aunque Voting y Bagging involucran múltiples modelos, Voting combina diferentes tipos de modelos y Bagging usa múltiples versiones del mismo tipo de [[modelo]].

