# go-project-setup

To download and install Go (Golang) on Ubuntu, you can follow these steps:

1. **Download the latest version of Go**:
   - First, visit the [official Go download page](https://golang.org/dl/) to find the URL for the latest version.
   - Use `wget` to download the .tar.gz file. Here’s an example with a specific version (replace `1.20.5` with the latest version if necessary):

     ```bash
     wget https://go.dev/dl/go1.20.5.linux-amd64.tar.gz
     ```

2. **Extract the tarball**:
   ```bash
   sudo tar -C /usr/local -xzf go1.20.5.linux-amd64.tar.gz
   ```

3. **Set up Go environment variables**:
   - Add Go binary to your PATH by editing the `.profile` file:

     ```bash
     nano ~/.profile
     ```

   - Add the following line at the end of the file:

     ```bash
     export PATH=$PATH:/usr/local/go/bin
     ```

   - Save and close the file (Ctrl + X, then Y, then Enter).

   - Apply the changes:

     ```bash
     source ~/.profile
     ```

4. **Verify the installation**:
   - Check the installed version to ensure Go is properly set up:

     ```bash
     go version
     ```

These steps will download, install, and configure Go on your Ubuntu system.
