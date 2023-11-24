---
layout: paper
categories: projects
permalink: projects/lib-dependency
id: lib-dependency
title: "Context-aware Reachability Analysis for Vulnerable Open-Source Libraries"

feature-title: "Vulnerability Analysis for Python Applications"
feature-description: "Rapid risk assessment technique that focuses on offline data preprocessing to simplify future online analysis, and reduce complexity of functional call graph to help prioritize vulnerability remediation."
# coming-soon: true
# year: 2023
# url: /projects/llmkg
# featured: false
# feature-order: 20230801
# selected: false
# type: project
# doi: 
---

We propose a method for rapid real time risk assessment in which we find relevant vulnerable versions and generate their functional call graphs. Functional call graphs are very large in size. These leads to scalability issues during analysis of large libraries. In languages like Python, where dynamic functions and paths are common, dynamic analysis is necessary to identify reachable paths. These paths cannot be detected during static analysis. This necessitates test case generation with appropriate inputs to identify these paths. It is also important to find exactly which functions generate these branches, as exhaustively targeting functions wastes resources and raises scalability problems. 

Function level pruning helps contain the complexity of the call graph. Clustering based on risk metrics is used to simplify future online analysis. This helps us generate rapid results and rank the libraries used in application based on the risk levels. 

