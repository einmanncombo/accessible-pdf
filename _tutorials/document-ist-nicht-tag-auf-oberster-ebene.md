---
ID: 176
post_title: '<em>Document</em> ist nicht Tag auf oberster Ebene'
author: Stefan Brechbühl
post_excerpt: 'Ein aus Word konvertiertes PDF enthält als oberster Container das &lt;Part&gt; Element. Für die oberste Strukturebene sollte jedoch das semantisch geeignetere &lt;Document&gt; Tag verwendet werden.'
layout: tutorials
permalink: >
  http://accessible-pdf.info/de/tutorials/document-ist-nicht-tag-auf-oberster-ebene/
published: true
post_date: 2018-01-05 16:24:27
tags:
  - manuelle Prüfung
  - Microsoft Word
categories:
  - 01. Getaggter realer Inhalt
---
## Problembeschreibung

Ein aus Word konvertiertes PDF enthält als oberster Container das `<Part>` Element. Für die oberste Strukturebene sollte jedoch das semantisch geeignetere `<Document>` Tag verwendet werden.

Problem wurde festgestellt bei der PDF-Konvertierung aus:

*   Microsoft Word 2013 für Windows

### PAC 2 Warnung

> Part structure element used as root element

### Prüfpunkt/e Matterhorn Protokoll

> **01-006** Der Strukturtyp und Attribute eines Strukturelementes sind nicht semantisch geeignet für das Strukturelement. Alle Strukturelemente müssen in Betracht gezogen werden. (→ [automatische Prüfung][1])

## Manueller Lösungsweg in Acrobat

Der oberste `<Part>` *Tag* muss in den `<Document>` *Tag* geändert werden, siehe dazu [„PDF-Tags in Acrobat ändern“][2].

 [1]: https://accessible-pdf.info/de/glossar/#automatische-pruefung
 [2]: https://accessible-pdf.info/de/basics/pdf-tags-in-acrobat-aendern/