## Fine-Tuning BGE Embeddings Using Synthetic Data from Amazon Bedrock

### Getting Started

This guide assumes you have already set up a SageMaker Studio environment as described in the blog post. Follow these steps to set up your environment and run the code:

1. Clone the repository:

   ```bash
   git clone https://github.com/aws-samples/finetune-bge-embeddings-blog.git
   cd finetune-bge-embeddings-blog
   ```

2. Create the Conda environment:

   ```bash
   conda env create -f environment.yml
   ```

   This step may take several minutes to complete.

3. Activate the environment:

   ```bash
   conda init
   source ~/.bashrc 
   conda activate ft-embedding-blog
   ```

4. Add the new Conda environment to Jupyter:

   ```bash
   python -m ipykernel install --user --name=ft-embedding-blog
   ```

5. Open the Jupyter notebook:
   - From the SageMaker Studio Launcher, open the repository folder named `finetune-bge-embeddings-blog`.
   - Open the file `finetune-bge-embeddings.ipynb`.

6. Select the correct kernel:
   - From the "Kernel" dropdown menu in the notebook, select "Change Kernel...".
   - Choose "ft-embedding-blog".
   - If you don't see the kernel, try refreshing your browser.

7. You're now ready to run the code in the notebook. Follow the instructions in each cell to generate synthetic data, fine-tune the BGE model, evaluate its performance, and deploy it using Amazon SageMaker.

Note: Make sure you have the necessary permissions and quotas set up in your AWS account to use Amazon Bedrock and SageMaker services as described in the blog post.

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.
