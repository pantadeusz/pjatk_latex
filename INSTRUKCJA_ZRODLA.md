# Źródła do tabel i rysunków

## Wytyczne PJATK
Każda tabela i rysunek musi mieć tytuł (bez kropki) i źródło (z kropką).

## Szybko: Makro \putimage
```latex
% Bez źródła
\putimage{Tytuł}{ścieżka/obraz}{fig:id}{0.5\textwidth}

% Ze źródłem
\putimage[opracowanie własne]{Tytuł}{ścieżka/obraz}{fig:id}{0.5\textwidth}

% Z cytowaniem
\putimage[\fullcite{KEY}]{Tytuł}{ścieżka/obraz}{fig:id}{0.5\textwidth}
```

## Długo: Środowisko figure

```latex
\begin{figure}[h!]
    \centering
    \includegraphics[width=0.5\textwidth]{ścieżka/obraz}
    \caption{Tytuł}
    \figuresource{opracowanie własne}
    \label{fig:id}
\end{figure}
```

Dla tabel użyj `\begin{table}...\tablesource{...}`.

## Przykłady źródeł

- `opracowanie własne`
- `opracowanie własne na podstawie KFT 2009`
- `\fullcite{BIBTEX_KEY}`
- `dostępne przez: http://example.com; 21.04.2025 r.`
