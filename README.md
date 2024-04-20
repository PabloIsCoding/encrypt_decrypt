# Encrypt and decrypt files or directories conveniently from the linux command line

Works on both files and directories (for directories, the `encrypt` script calls `tar` first and then `gpg`, while for files it's just `gpg`).

**IMPORTANT: These scripts will remove your original files or directories (if the encryption/decryption was succesful). Make sure to make copies before using it the first time, just in case it works differently on your machine for some odd reason. Also make sure that you understand the code. There is a video explaining how the scripts work so that you can see for yourself what they do.**

[Youtube video](https://www.youtube.com/watch?v=T32WxI_IHsc)

## Install

Just download the two scripts and throw them in your `~/bin/` or your `~/.local/bin/` or wherever you put your programs.

## Usage

```bash
$ encrypt some_file_or_dir
$ decrypt some_file_or_dir.gpg
```

You can also use wildcards like, for example:

```bash
$ encrypt *.png
$ decrypt *.png.gpg
```

If you want to encrypt several files into a single gpg file, put them into a directory first. Otherwise, it'll ask you to type the password once per file/dir.
