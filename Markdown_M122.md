# M122

**Erstellt am:** 18. September 2025, 10:22 Uhr

Heute habe ich am Anfang der Lektion das Quiz gemacht und danach mit dem der installation von VSC und deren Extensions angefangen. Danach habe ich VSC ein bisschen getestet und als ich dies hatte, habe ich angefangen auf VSC Markdown eine art von OneNote zu machen.
Jetzt versuche ich gerade, dieses Dokument/File.md mit dem GitHub repository zu verbinden.

---

**Erstellt am:** 19. September 2025, 15:15 Uhr

Ich habe gerade verscuht mein Markdwon file mit GitHub repository zu verbinden und habe es geschafft. Dabei habe ich GitHub Copilot benutzt für die Hilfe.
Ich musste zuerst Git installieren und dann VSC neustarten.![GIT-Immage_exe](image.png)

Danach musste ich VSC mit GitHUb verbinden. Als ich dies hatte wurde noch ein ".gitignore" file erstellt und musste dann mein Markdown file dort hinzufügen, in dem ich in das Terminal gehe und "git commit -m "Track Markdown_M122.md and update .gitignore"" eingebe.  Danach musste ich "git branch" eingeben und es muss dann "main" angezeigt werden, dies geschiet auch. Als ich dies hatte konnte ich dann "git push origin main" eingeben, weil mein Branch "main" ist. Leider hatte dies nicht geklappt und musste "git remote add origin https://github.com/Sweazyyy881/Public.git" eingeben und dann noch "git push -u origin main". Als ich dies hatte wurde dies auf GitHub transferiert und hatte somit die Verbindung. Jetzt habe ich auf Github geschaut und es hat funktioniert, siehe Bild.

![Repository-Public_Image](image-1.png)

GitHub Repository Link: Sweazyyy881/Public

Mit diesem Commands kann man die Datei auf GitHub wieder hochladen, wenn man an der Datei gearbeitet hat.
Code

git add <dateiname.md>
git commit -m "Markdown_M122.md"
git push
