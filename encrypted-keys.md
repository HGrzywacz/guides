Encryption with `encfs`
======================

To see encypted files mount folder with encfs:

  ```sh
  $ encfs ~/.encrypted-keys/ ~/encrypted-keys/
  ```

To umount:

  ```sh
  $ fusermount -u encrypted-keys
  ```


Following this [Ubuntu documentation](https://help.ubuntu.com/community/FolderEncryption)
