<p align="center">
  <img src="Networks-Unmasked-Definitive-Edition-cover.png" alt="Networks Unmasked — Definitive Edition cover, original artwork by Emil Valiyev" width="310">
</p>

<h1 align="center">Networks Unmasked</h1>
<p align="center"><em>How Data Travels, What It Reveals, and the Cost of Privacy</em></p>
<p align="center">Emil Valiyev &nbsp;·&nbsp; Definitive Edition &nbsp;·&nbsp; 26 October 2026</p>

<p align="center">
  <a href="https://github.com/emillvl/networks-unmasked/releases/download/v1.0.0/Networks-Unmasked-Definitive-Edition.pdf"><strong>Download the book (PDF)</strong></a>
  &nbsp;·&nbsp;
  <a href="https://leanpub.com/networks-unmasked">Leanpub</a>
  &nbsp;·&nbsp;
  <a href="https://doi.org/10.6084/m9.figshare.34792464.v1">Figshare / DOI</a>
  &nbsp;·&nbsp;
  <a href="https://zenodo.org/records/23671687">Zenodo</a>
</p>

---

## About the book

A web page is the visible end of a long chain of decisions. Before it appears, a computer has resolved a name, chosen a route, exchanged packets, and established how to communicate with another machine. Most of that work happens out of sight. So does much of the information it reveals.

*Networks Unmasked* follows that journey, from the hardware moving bits to the systems that try to conceal where traffic comes from and where it goes. The central question is straightforward: **what can be hidden, what remains visible, and how much performance does privacy cost?**

The book builds its explanations from first principles. It does not assume formal computer science training, but it does take the machinery seriously: network interfaces and memory buffers, routing decisions and address translation, sockets and transport protocols, encryption, name resolution, and the boundaries of anonymity networks.

## Inside

The 22 chapters follow one continuous line of reasoning:

| Chapters | What they cover |
| --- | --- |
| **1–5 · The path** | How a message leaves an application, moves through the host, reaches neighbors and routers, and finds a destination by name. |
| **6–8 · The conversation** | Sockets, ports, UDP, TCP, and the application protocols that shape what crosses the network. |
| **9–14 · Exposure and protection** | What observers can learn, how traffic can be intercepted or manipulated, what encrypted channels protect, and how DNS protections, firewalls, proxies, tunnels, and VPNs change the picture. |
| **15–18 · Anonymity networks** | How Tor and I2P work, where their boundaries lie, and what trust and performance costs their designs introduce. |
| **19–22 · Engineering the boundary** | Lifecycle failures, honest performance measurement, optimization without weakening confinement, and the limits of practical traffic masking. |

Two appendices trace a request through the complete machine and explain how to read and extend the evidence. The book closes with its technical references.

## From mechanisms to working systems

The engineering examples come from [Ghostnector](https://github.com/emillvl/Ghostnector), my Linux network-privacy project.

Ghostnector is not presented as a magic switch for anonymity. Its development produced the kinds of problems that diagrams tend to hide: filtering and address-translation rules interacting in the wrong order, configuration exceptions matching the wrong packet fields, protections that must remain in place during startup and shutdown, and performance figures that need careful interpretation.

Those cases give the book something concrete to test its explanations against. They also show why a configuration that *looks* correct is not enough: effective kernel policy, real packet paths, and transitions between states matter.

The distinction between **source inspection, documented test reports, and independently reconstructed measurements** is deliberate. An observed result in one system is not a promise about every machine or future version. The book and Ghostnector are separate works.

## Reading and editions

The **Definitive Edition (v1.0)** is a 108-page PDF, published on **26 October 2026**. It includes original explanatory diagrams and an evidence trail tied to Ghostnector commit `17a03c4` and technical sources consulted through **24 October 2026**.

- **[Download the definitive PDF](https://github.com/emillvl/networks-unmasked/releases/download/v1.0.0/Networks-Unmasked-Definitive-Edition.pdf)** — the complete book.
- **[GitHub release](https://github.com/emillvl/networks-unmasked/releases/tag/v1.0.0)** — edition files and checksum.
- **[Leanpub](https://leanpub.com/networks-unmasked)** — book listing.
- **[Figshare](https://doi.org/10.6084/m9.figshare.34792464.v1)** — citable edition record and DOI.
- **[Zenodo](https://zenodo.org/records/23671687)** — archival copy using the same edition identifier.

If you're reading this to learn networking, begin at Chapter 1: each section introduces the concepts the later chapters rely on. If you already know the fundamentals, the table of contents will take you directly to the privacy systems, engineering cases, and measurements.

## Citation

> Valiyev, Emil. (2026). *Networks Unmasked: How Data Travels, What It Reveals, and the Cost of Privacy*. Definitive Edition, version 1.0. https://doi.org/10.6084/m9.figshare.34792464.v1

The repository also includes [`CITATION.cff`](CITATION.cff) for citation tools and GitHub's **Cite this repository** feature.

<details>
<summary>Verify your PDF</summary>

The published PDF's SHA-256 checksum is:

```text
f94b9d97b49ec6bc94db2f856b8199c6e4282bab561317f7980e7c1ee5608905
```

See [`SHA256SUMS`](SHA256SUMS) for the file name and checksum.

</details>

## Authorship and license

Text and original artwork by **Emil Valiyev**. AI assisted with a final editorial audit of wording, spelling, organization, and structural consistency.

Copyright © 2026 Emil Valiyev. The book's text and original artwork are licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE). Referenced third-party works and the Ghostnector software remain subject to their respective licenses.
