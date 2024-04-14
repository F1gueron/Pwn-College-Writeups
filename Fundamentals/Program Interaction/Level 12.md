Make a script to get the flag  

```bash
echo "{{given_password}}" > {{given_location}}
echo "/challenges/embryoio_level12 < {{given_location}}" > /tmp/my_script.sh
bash /tmp/my_script.sh
