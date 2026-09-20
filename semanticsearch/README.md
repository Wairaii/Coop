# Semantic Search Experiments

Jupyter notebooks for experimenting with multilingual semantic search over job and resume data using ChromaDB and Sentence Transformers.

## Setup

1. Create and activate a Python virtual environment.
2. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Start or connect to a ChromaDB server. The notebooks read these environment variables:

   - `CHROMA_HOST` (default: `localhost`)
   - `CHROMA_PORT` (default: `8000`)

4. Place required local datasets, such as `jobs_search_master.csv`, in this directory when a notebook references them.
5. Start Jupyter Lab and run the relevant notebook.

## Notebooks

- `create_collection.ipynb`: creates and populates ChromaDB collections with multilingual embedding models.
- `job_search_test.ipynb`: ingests job data and exercises local semantic job queries.
- `all_job_test_querry.ipynb`: runs broader job-query experiments.
- `jobs_search_master_test.ipynb`: tests the main job-search collection.
- `member_resume_search_master_test.ipynb`: tests semantic search over member resumes.
- `auto_complete_test.ipynb`: explores autocomplete behavior with notebook widgets.
- `test_db.ipynb`: inspects collections and runs database search experiments.

Notebook outputs are cleared before publishing so test data is not committed.
