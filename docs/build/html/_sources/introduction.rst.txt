Introduction
=============
    This document describes the Little Hill Lab's initial requirements for an online
    application (Oh My Genes) which allows our scientists to upload gene expression files
    and quickly get differentially expressed genes.


Purpose
--------
    To identify differentially expressed genes given a gene expression file containing
    two cell samples.


Overview
---------
    The web application has a simple interface with a single button **[Upload and GO]**. Our
    scientists upload a plain text file containing gene expression levels from two samples,
    representing two experimental conditions. Accepting the file, the software will return a table
    of differentially expressed genes and a scatter plot of these genes whose X-axis is control and
    Y-axis is treatment. If an invalid gene expression is given, the web application returns a page
    informing the user to provide the correct format.

.. image:: /image/1.png




Client
-------
    Biologists in Little Hill Laboratory.


Domain knowledge
----------------
    **Control sample** - a cell sample prepared in its normal condition.

    **Treatment sample** - a cell sample treated by special chemicals, or in which some genes
    are altered.

    **Differentially expressed genes** - the genes which have significantly different
    expression levels between two samples.

    **Up-regulation** - a gene is said to be up-regulated if it has higher expression in
    treatment than in control.

    **logFC** - log fold change of gene expression. log_2 [T/C], where T is the gene
    expression level from a treatment sample, while C is the gene expression level from a
    control sample.
