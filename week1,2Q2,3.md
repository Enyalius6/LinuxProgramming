Q2)
read c
read a b
fileco=$(sed -n "${a},{b}p" "$c")
echo "$fileco"


Q3)
read c
read s
d="temp.txt"
fileco=$(grep -v "${s}" ${c}>${d})
mv "$d" "$c"
cat "$c"
