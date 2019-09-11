# dot

## setup

```
git clone https://github.com/mbigras/dot
cd dot
vagrant up
ansible -i vagrant.yml all -m ping
ansible-playbook -i vagrant.yml dot.yml
vagrant ssh dot
cd /vagrant/
cat <<'EOF' | dot -Tpng -o graph1.png
digraph G {
	foo -> bar -> baz;
	foo -> bat;
	foo -> cat;
	baz -> cow;
	baz -> ant;
	bat -> bow;
	foo -> flap;
	baz -> apple;
}
EOF
```
