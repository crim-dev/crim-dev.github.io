---
layout: post
title:  "Welcome to Jekyll!"
date:   2024-10-16 10:10:21 +0200
categories: jekyll update
---

<u>Définition : (primitive)</u>
$$
\begin{align}
&f:I\to \mathbb{R} \text{ continue} \\
&F \text{ s'appelle une primitive de } f \text{ si } F \text{ est dérivable et } F'=f \text{ sur I}
\end{align}
$$<u>Réciproque</u>
$$
\begin{align}
&\text{Si } f:I\to \mathbb{R} \text{ continue avec pour primitive } F \text{, alors l'ensemble de toutes les primitives est } \\
&\{F+C | C \in \mathbb{R}\}
\end{align}

$$
$$
\begin{align}
&\text{Soient } F, G \text{ primitives de } f \text{ sur } I. \\
&(F-G)'=F'-G'=f-f=0 \text{ sur } I. \\
&\implies (F-G)(x)=C, \forall x \in I
\end{align}

$$

<u>Théorème</u> (existence d'une primitive)
$$
\text{Si } f:I\to \mathbb{R} \text{ est continue, il existe une primitive } F:I\to\mathbb{R}
$$
En vue de la proposition pour $a,b \in I$ la valeur de $F(b)-F(a)$ ne dépend pas du choix de primitive
$$
\begin{align}
F(b)-F(a) &= G(b)+C-[G(a)+C] \\
&= G(b) -G(a)
\end{align}
$$
$$
G(x)=F(x)+C
$$
On peut alors définir **l'intégrale de f entre a et b** : 
<u>Définition</u>
$$
\begin{align}
&f:I \to \mathbb{R} \text{ continue, avec pour primitive } F:I\to \mathbb{R} \text{ },a,b \in \mathbb{R} \\
&\int_{a}^b f(x)dx := F(b)-F(a)
\end{align}
$$
<u>Notation</u>

$$
\begin{align}
&\int f(x)dx = \text{ primitive générale } \\
&F(x)-F(a)=\int_{a}^xf(t)dt= \text{ primitive qui s'annule en a}
\end{align}

$$

<u>Exemples</u>

$$
\begin{align}
&\text{1) } f:\mathbb{R}\to \mathbb{R}, f(x)=x^n \\
&F(x)=\frac{1}{n+1}x^{n+1}, n\neq -1 \\
&\text{ car } F'(x)=\frac{1}{n+1}(n+1)x^n=x^n  \\
\end{align}
$$

$$
\begin{align}
&\text{2) } f:\mathbb{R}\to \mathbb{R}, f(x)= \cos(x) \\
&F(x)=\sin(x) \text{ est une primitive de f} \\
&F'(x) = \cos(x) \text{ sur } \mathbb{R}
\end{align}

$$
$$
\begin{align}
&\text{3) } f:\mathbb{R}_{+}\to \mathbb{R}, f(x) =\ln(x) \\
&F(x)=x\ln(x)-x,F:\mathbb{R}_{+}\to \mathbb{R} \\
&F'(x)=(x\ln x)'-1=x \cdot \frac{1}{x}+\ln(x)-1=\ln(x)
\end{align}
$$
<u>Propriété de l'intégrale</u>
<u>i) Relation de Chasles</u>
$$
\int_{a}^b f(t)\,dt=\int_{a}^if(t)\,dt+\int_{i}^b f(t)\,dt
$$
<u>ii) Linéarité</u>
$$
\int_{a}^{b} (f+\lambda g)(t) \, dt = \int_{a}^{b} f(t) \, dt + \lambda \int_{a}^{b} g(t) \, dt, \forall \lambda \in \mathbb{R}  
$$
<u>iii) Positivité et comparaison</u>
$$
\text{Si } a < b: f\geq 0 \text{ sur } [a;b]
\implies \int_{a}^{b} f(t) \, dt \geq 0 
$$

$$
\int_{a}^b f(t) \, dt
$$

<u>Changement de variables</u>

$$
\int_{a}^{b} f'(g(x))g'(x) \, dx = \int_{g(a)}^{g(b)} f(x) \, dx 
$$

Exemple : 
$$
\begin{align}
\int \tanh(x) \,dx = \int \frac{\sinh(x)}{\cosh(x)}\,dx
\end{align}

$$
