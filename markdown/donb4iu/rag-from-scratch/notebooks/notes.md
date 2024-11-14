# RAG From Scratch

LLMs are trained on a large but fixed corpus of data, limiting their ability to reason about private or recent information. Fine-tuning is one way to mitigate this, but is often [not well-suited for facutal recall](https://www.anyscale.com/blog/fine-tuning-is-for-form-not-facts) and [can be costly](https://www.glean.com/blog/how-to-build-an-ai-assistant-for-the-enterprise).
Retrieval augmented generation (RAG) has emerged as a popular and powerful mechanism to expand an LLM's knowledge base, using documents retrieved from an external data source to ground the LLM generation via in-context learning. 
These notebooks accompany a [video playlist](https://youtube.com/playlist?list=PLfaIDFEXuae2LXbO1_PKyVJiQ23ZztA0x&feature=shared) that builds up an understanding of RAG from scratch, starting with the basics of indexing, retrieval, and generation. 
![rag_detail_v2](https://github.com/langchain-ai/rag-from-scratch/assets/122662504/54a2d76c-b07e-49e7-b4ce-fc45667360a1)
 
**_Modified to work with OLLAMA models._**


## Reference

- [Learn RAG From Scratch – Python AI Tutorial from a LangChain Engineer](https://www.youtube.com/watch?v=sVcwVQRHIc8)


## Environment

```
(base) #( 10/22/24@ 6:04PM )( donbuddenbaum@donbs-imac ):~/documents
   conda create --name ragfs python=3.12

Channels:
 - defaults
Platform: osx-64
Collecting package metadata (repodata.json): done
Solving environment: done

## Package Plan ##

  environment location: /Users/donbuddenbaum/anaconda3/envs/ragfs

  added / updated specs:
    - python=3.12


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    ca-certificates-2024.9.24  |       hecd8cb5_0         131 KB
    expat-2.6.3                |       h6d0c2b6_0         151 KB
    openssl-3.0.15             |       h46256e1_0         4.5 MB
    pip-24.2                   |  py312hecd8cb5_0         2.8 MB
    python-3.12.7              |       hcd54a6c_0        14.0 MB
    setuptools-75.1.0          |  py312hecd8cb5_0         2.2 MB
    tzdata-2024b               |       h04d1e81_0         115 KB
    wheel-0.44.0               |  py312hecd8cb5_0         146 KB
    ------------------------------------------------------------
                                           Total:        24.0 MB

The following NEW packages will be INSTALLED:

  bzip2              pkgs/main/osx-64::bzip2-1.0.8-h6c40b1e_6
  ca-certificates    pkgs/main/osx-64::ca-certificates-2024.9.24-hecd8cb5_0
  expat              pkgs/main/osx-64::expat-2.6.3-h6d0c2b6_0
  libcxx             pkgs/main/osx-64::libcxx-14.0.6-h9765a3e_0
  libffi             pkgs/main/osx-64::libffi-3.4.4-hecd8cb5_1
  ncurses            pkgs/main/osx-64::ncurses-6.4-hcec6c5f_0
  openssl            pkgs/main/osx-64::openssl-3.0.15-h46256e1_0
  pip                pkgs/main/osx-64::pip-24.2-py312hecd8cb5_0
  python             pkgs/main/osx-64::python-3.12.7-hcd54a6c_0
  readline           pkgs/main/osx-64::readline-8.2-hca72f7f_0
  setuptools         pkgs/main/osx-64::setuptools-75.1.0-py312hecd8cb5_0
  sqlite             pkgs/main/osx-64::sqlite-3.45.3-h6c40b1e_0
  tk                 pkgs/main/osx-64::tk-8.6.14-h4d00af3_0
  tzdata             pkgs/main/noarch::tzdata-2024b-h04d1e81_0
  wheel              pkgs/main/osx-64::wheel-0.44.0-py312hecd8cb5_0
  xz                 pkgs/main/osx-64::xz-5.4.6-h6c40b1e_1
  zlib               pkgs/main/osx-64::zlib-1.2.13-h4b97444_1


Proceed ([y]/n)? y


Downloading and Extracting Packages:

Preparing transaction: done
Verifying transaction: done
Executing transaction: done
#
# To activate this environment, use
#
#     $ conda activate ragfs
#
# To deactivate an active environment, use
#
#     $ conda deactivate

(base) #( 10/22/24@ 6:07PM )( donbuddenbaum@donbs-imac ):~/documents
   conda activate ragfs

(ragfs) #( 10/22/24@ 6:07PM )( donbuddenbaum@donbs-imac ):~/documents
```