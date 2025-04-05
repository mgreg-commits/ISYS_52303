1. **Set Python Version**

  ```cmd

  pyenv install 3.10.4

  pyenv local 3.10.4

  ```

  Note: The first command might take a few minutes to complete



2. **Create and Activate Virtual Environment**

  ```cmd

  python -m venv timexer-env

  timexer-env\Scripts\activate

  ```

  Your command prompt should now show `(timexer-env)` at the beginning



3. **Install Dependencies-The debuged code is in the TimeXer folder**

  ```cmd

  cd TimeXer

  pip install -r requirements.txt

  pip install --upgrade einops

  

  :: Install PyTorch with CUDA support

  pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu124

  ```

  Note: These installations might take several minutes



4. **Set GPU Device** (if you have multiple GPUs)

  ```cmd

  set CUDA_VISIBLE_DEVICES=0

  ```



5. **Run TimeXer**

  ```cmd

  TimeXer.bat

  ```