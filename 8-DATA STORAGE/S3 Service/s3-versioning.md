
# Enable Versioning at Object level
- Protection against accidental delete
- Protection against accidental overwrites
- Delete marker is created for that object
- If u delete with the version ID, s3 removes the version as well
- With constant overrides, we accumulate non-current versions of the object
- You can use life-cycle to delete non-current versions after a period of time in days