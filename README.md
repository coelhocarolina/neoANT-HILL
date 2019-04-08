# neoANT-HILL

neoANT-HILL is a python toolkit that integrates several pipelines for fully automated identification of potential neoantigens (pNeoAgs) which could be used in personalized immunotherapy due to their ability to elicit and boosting T-cell immune response. It is available as a Docker pre-built image and allows the analysis of single- or multiple samples. As input files is required RNA sequencing reads and/or somatic DNA mutations derived from Next Generating Sequencing.


<h2><a id="user-content-installation-pip" class="anchor" aria-hidden="true" href="#installation-pip"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>1. Requirements </h2>

<h2><a id="user-content-installation-pip" class="anchor" aria-hidden="true" href="#installation-pip"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>2. Installation </h2>

<pre><code>$ docker build -t neoanthill:1.0 /path/to/Dockerfile
</code></pre>

<p>Running the container:</p>

<pre><code>$ docker run -v path/to/input:/home/biodocker/input -v path/to/output:/home/biodocker/output -p 8000:80 -it neoanthill:1.0 /bin/bash
</code></pre>

