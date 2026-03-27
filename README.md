\documentclass[11pt]{article}

% Packages for formatting and links
\usepackage[utf8]{inputenc}
\usepackage[margin=1in]{geometry}
\usepackage{graphicx}
\usepackage{hyperref}
\usepackage{listings}
\usepackage{xcolor}
\usepackage{titlesec}

% Setup code listing styles
\lstset{
    backgroundcolor=\color{gray!10},
    basicstyle=\ttfamily\small,
    breaklines=true,
    frame=single,
    keywordstyle=\color{blue},
    language=Python
}

% Hyperlink styling
\hypersetup{
    colorlinks=true,
    linkcolor=blue,
    urlcolor=cyan,
    pdftitle={Plant Disease Recognition README}
}

\title{\textbf{Plant Disease Recognition System}}
\author{Deep Learning Project Documentation}
\date{\today}

\begin{document}

\maketitle

\section{Overview}
The Plant Disease Recognition System is a deep learning-based application designed to identify 38 different classes of plant diseases from leaf images. The system utilizes a Convolutional Neural Network (CNN) and provides a web-based interface for real-time inference.

\section{Features}
\begin{itemize}
    \item \textbf{High Accuracy:} Achieves approximately 95\% accuracy on the test dataset.
    \item \textbf{Streamlit UI:} User-friendly web dashboard for image uploads and results.
    \item \textbf{Comprehensive Coverage:} Detects diseases in crops including Tomato, Potato, Apple, Corn, and Grapes.
    \item \textbf{End-to-End Pipeline:} Covers everything from data preprocessing and training to deployment.
\end{itemize}

\section{Project Architecture}
The project consists of the following core components:
\begin{description}
    \item[\texttt{main.py}] The Streamlit application entry point.
    \item[\texttt{trained\_model.keras}] Pre-trained CNN model saved in Keras format.
    \item[\texttt{Train\_plant\_disease.ipynb}] Notebook containing the training logic and architecture.
    \item[\texttt{Test\_plant\_disease.ipynb}] Notebook for model evaluation and metrics.
    \item[\texttt{training\_hist.json}] JSON file storing training/validation loss and accuracy history.
\end{description}

\section{Installation}
To set up the environment, ensure you have Python installed and run the following:

\begin{lstlisting}[language=bash]
# Install required libraries
pip install streamlit tensorflow numpy matplotlib pandas seaborn
\end{lstlisting}

\section{Usage}
To launch the recognition system, navigate to the project directory and execute:

\begin{lstlisting}[language=bash]
streamlit run main.py
\end{lstlisting}

\section{Model Performance}
The model was trained on the \textit{New Plant Diseases Dataset} from Kaggle.
\begin{itemize}
    \item \textbf{Model Architecture:} Sequential CNN with Max-Pooling and Dropout.
    \item \textbf{Input Shape:} $128 \times 128 \times 3$ (RGB).
    \item \textbf{Final Validation Accuracy:} ~95\%.
\end{itemize}

\section{Dataset Reference}
The dataset used for this project can be found on Kaggle: \\
\url{https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset}

\end{document}
