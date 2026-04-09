# Récap maths — Sigma, Log, Lim, e

---

## Σ — La Somme (Sigma)

### Notation

$$\sum_{i=a}^{b} f(i) = f(a) + f(a+1) + \cdots + f(b)$$

### Exemples

$$\sum_{i=1}^{4} i = 1 + 2 + 3 + 4 = 10$$

$$\sum_{i=1}^{4} i^2 = 1^2 + 2^2 + 3^2 + 4^2 = 30$$

$$\sum_{i=0}^{3} 2^i = 1 + 2 + 4 + 8 = 15$$

### Formules fermées

$$\sum_{i=1}^{n} i = \frac{n(n+1)}{2}$$

$$\sum_{i=1}^{n} i^2 = \frac{n(n+1)(2n+1)}{6}$$

$$\sum_{i=1}^{n} i^3 = \left(\frac{n(n+1)}{2}\right)^2$$

$$\sum_{i=0}^{n} r^i = \frac{1 - r^{n+1}}{1 - r} \quad \text{avec } r \neq 1$$

### Propriétés

$$\sum_{i=1}^{n} (f(i) + g(i)) = \sum_{i=1}^{n} f(i) + \sum_{i=1}^{n} g(i)$$

$$\sum_{i=1}^{n} c \cdot f(i) = c \cdot \sum_{i=1}^{n} f(i)$$

$$\sum_{i=1}^{n} c = n \cdot c$$

---

## Π — Le Produit (Pi majuscule)

### Notation

$$\prod_{i=a}^{b} f(i) = f(a) \times f(a+1) \times \cdots \times f(b)$$

### Exemple

$$\prod_{i=1}^{4} i = 1 \times 2 \times 3 \times 4 = 24$$

### Lien avec la factorielle

$$n! = \prod_{i=1}^{n} i$$

$$0! = 1 \quad \text{(par convention)}$$

$$\binom{n}{k} = \frac{n!}{k!(n-k)!} \quad \text{(combinaisons)}$$

---

## log — Le Logarithme

### Définition fondamentale

$$\log_b(x) = y \iff b^y = x$$

### Les 3 bases principales

| Notation | Base | Définition |
|---|---|---|
| $\log_2(x)$ | $2$ | $\log_2(x) = y \iff 2^y = x$ |
| $\log_{10}(x)$ | $10$ | $\log_{10}(x) = y \iff 10^y = x$ |
| $\ln(x)$ | $e \approx 2.718$ | $\ln(x) = y \iff e^y = x$ |

### Valeurs à connaître

$$\log_b(1) = 0 \quad \forall b$$

$$\log_b(b) = 1 \quad \forall b$$

$$\log_b(b^n) = n$$

$$\ln(e) = 1 \quad \ln(1) = 0 \quad \ln(e^n) = n$$

### Propriétés (valables pour toute base)

$$\log(a \times b) = \log(a) + \log(b)$$

$$\log\left(\frac{a}{b}\right) = \log(a) - \log(b)$$

$$\log(a^n) = n \cdot \log(a)$$

$$\log(\sqrt{a}) = \frac{1}{2} \log(a)$$

$$\log_b(a) = \frac{\ln(a)}{\ln(b)} \quad \text{(changement de base)}$$

### Domaine et comportement

$$\ln(x) \text{ défini uniquement pour } x > 0$$

$$\ln(x) < 0 \quad \text{si } 0 < x < 1$$

$$\ln(x) = 0 \quad \text{si } x = 1$$

$$\ln(x) > 0 \quad \text{si } x > 1$$

---

## e — La constante d'Euler

### Définition par la limite

$$e = \lim_{n \to +\infty} \left(1 + \frac{1}{n}\right)^n \approx 2.71828182845\ldots$$

### Définition par la série

$$e = \sum_{n=0}^{+\infty} \frac{1}{n!} = 1 + 1 + \frac{1}{2} + \frac{1}{6} + \frac{1}{24} + \cdots$$

### La fonction exponentielle

$$e^x = \sum_{n=0}^{+\infty} \frac{x^n}{n!}$$

$$e^0 = 1 \quad e^1 = e \quad e^{-x} = \frac{1}{e^x}$$

$$e^{a+b} = e^a \times e^b$$

### Lien avec ln (fonctions inverses)

$$\ln(e^x) = x \quad \forall x \in \mathbb{R}$$

$$e^{\ln(x)} = x \quad \forall x > 0$$

---

## lim — La Limite

### Notation

$$\lim_{x \to a} f(x) = L$$

### Limites fondamentales

$$\lim_{x \to +\infty} \frac{1}{x} = 0 \qquad \lim_{x \to 0^+} \frac{1}{x} = +\infty$$

$$\lim_{x \to +\infty} e^x = +\infty \qquad \lim_{x \to -\infty} e^x = 0$$

$$\lim_{x \to +\infty} \ln(x) = +\infty \qquad \lim_{x \to 0^+} \ln(x) = -\infty$$

$$\lim_{x \to +\infty} x^n = +\infty \quad (n > 0)$$

### Limites remarquables

$$\lim_{x \to 0} \frac{\sin(x)}{x} = 1$$

$$\lim_{x \to 0} \frac{e^x - 1}{x} = 1$$

$$\lim_{x \to 0} \frac{\ln(1+x)}{x} = 1$$

$$\lim_{x \to +\infty} \frac{\ln(x)}{x} = 0$$

$$\lim_{x \to +\infty} \frac{x^n}{e^x} = 0 \quad \text{(l'expo écrase tout)}$$

### Formes indéterminées

Ces formes ne se calculent pas directement, il faut ruser :

$$\frac{0}{0} \quad \frac{\infty}{\infty} \quad 0 \times \infty \quad \infty - \infty \quad 0^0 \quad 1^\infty \quad \infty^0$$

### Règles de calcul

$$\lim_{x \to a} (f + g)(x) = \lim f + \lim g$$

$$\lim_{x \to a} (f \times g)(x) = \lim f \times \lim g$$

$$\lim_{x \to a} \frac{f}{g}(x) = \frac{\lim f}{\lim g} \quad \text{si } \lim g \neq 0$$

---

## Comparaison des croissances

De la plus lente à la plus rapide quand $x \to +\infty$ :

$$\ln(x) \ll x^a \ll e^x \ll x^x \quad (a > 0)$$

Ce qui implique :

$$\lim_{x \to +\infty} \frac{\ln(x)}{x} = 0 \qquad \lim_{x \to +\infty} \frac{x^{100}}{e^x} = 0$$

---

## Formules combinées utiles

### Moyenne

$$\bar{x} = \frac{1}{n} \sum_{i=1}^{n} x_i$$

### Variance

$$\sigma^2 = \frac{1}{n} \sum_{i=1}^{n} (x_i - \bar{x})^2$$

### Intérêts composés (finance)

$$A = P \cdot e^{rt} \qquad t_{\text{doublement}} = \frac{\ln(2)}{r}$$

### Désintégration radioactive

$$N(t) = N_0 \cdot e^{-\lambda t} \qquad t_{1/2} = \frac{\ln(2)}{\lambda}$$

### Entropie de Shannon (information / ML)

$$H = -\sum_{i=1}^{n} p_i \cdot \log_2(p_i)$$

### Log-vraisemblance (stats / ML)

$$\mathcal{L} = \sum_{i=1}^{n} \ln(p(x_i))$$

### Neurone artificiel (réseau de neurones)

$$\text{sortie} = f\left(\sum_{i=1}^{n} w_i \cdot x_i + b\right)$$

où $w_i$ sont les poids, $x_i$ les entrées et $b$ le biais.

---

## Ensembles de nombres

| Symbole | Nom | Contenu |
|---|---|---|
| $\mathbb{N}$ | Entiers naturels | $0, 1, 2, 3, \ldots$ |
| $\mathbb{Z}$ | Entiers relatifs | $\ldots, -2, -1, 0, 1, 2, \ldots$ |
| $\mathbb{Q}$ | Rationnels | $\frac{p}{q}$ avec $p, q \in \mathbb{Z}$ |
| $\mathbb{R}$ | Réels | Tous les nombres sur la droite |
| $\mathbb{C}$ | Complexes | $a + bi$ avec $i^2 = -1$ |

$$\mathbb{N} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R} \subset \mathbb{C}$$

---

## Quantificateurs logiques

| Symbole | Lecture | Sens |
|---|---|---|
| $\forall$ | "pour tout" | vrai pour chaque élément |
| $\exists$ | "il existe" | vrai pour au moins un |
| $\nexists$ | "il n'existe pas" | faux pour tous |
| $\in$ | "appartient à" | est un élément de |
| $\notin$ | "n'appartient pas" | n'est pas un élément de |

**Exemples :**

$$\forall x \in \mathbb{R},\ x^2 \geq 0$$

$$\exists x \in \mathbb{R},\ x^2 = 2 \quad (x = \sqrt{2})$$

$$\forall x > 0,\ \ln(x) \text{ est défini}$$
