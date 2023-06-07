# s1.03-s2.03

> s1.03 réalisé par Adélaïde Matéo, Aoulad-Tayab Karim
> s2.03 réalisé par Wasson Baptiste, Lagache Kylian, Aoulad-Tayab Karim

Les SaÉ en lien avec l'installation/configuration d'une machine sous Linux, plus particulièrement sous GNU/Linux Debian.

Vous pouvez consulter:
- [Le rapport en anglais de s1.03](anglais/the_debian_manual_for_rookies_ADELAIDE_AOULADTAYAB.pdf)
- [Le rapport final de la s2.03](rapport-final.pdf)

## Quelques détails sur la compilation du rapport de la s2.03...

La compilation HTML, PDF comprend:
- La génération automatique de la table des matières (avec ``--toc``).
- L'amélioration de l'aspect visuel via des templates (cf: [easy-pandoc-templates](https://github.com/ryangrose/easy-pandoc-templates)) stockés dans le répértoire ``template``

#### Compilation Markdown -> PDF

```
pandoc --toc -t pdf -f markdown-implicit_figures rapport-final.md -o rapport-final.pdf
```

#### Compilation Markdown -> HTML

```
pandoc --toc --template=template/easy_template.html -t html -f markdown rapport-final.md -o rapport-final.html
```