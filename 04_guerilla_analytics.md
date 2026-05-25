# Guerilla Analytics
## opdracht 3a
In deze opdracht heb ik de Guerrilla Analytics‑principes toegepast op de RNA‑sequencing formatieve opdracht uit de DAUR2‑module. Omdat de originele bestanden op de server staan, heb ik lokaal een projectmap aangemaakt en daarin lege bestanden met dezelfde bestandsnamen geplaatst (FASTQ, BAM, count‑tabellen, enz.). Op basis daarvan heb ik een GA‑proof mapstructuur ingericht, waarbij ruwe data, afgeleide data, code, documentatie en output strikt van elkaar gescheiden zijn.

Daarnaast heb ik een README‑bestand opgesteld waarin ik de inhoud van elke map, de herkomst van de data en de gebruikte conventies documenteer. Hieronder staan de vereiste screenshots:
<br>

- de mapstructuur gegenereerd met fs::dir_tree()

- de inhoud van het README‑bestand.



``` r
library(png)
library(grid)
library(gridExtra)
library(here)
```

```
## here() starts at C:/Users/Boste/OneDrive/Documenten/dsfb2_workflows_portfolio
```

``` r
img1 <- rasterGrob(as.raster(readPNG(here::here("images", "dirtree_daur2_formatief.png"))))
img2 <- rasterGrob(as.raster(readPNG(here::here("images", "readme_daur2_formatief.png"))))

grid.arrange(img1, img2, ncol=2, top=textGrob("Mapstructuur volgens Guerilla Analytics", gp=gpar(fontsize=10,font=8)))
```

<div class="figure">
<img src="04_guerilla_analytics_files/figure-html/opdracht 3a-1.png" alt="Mapstructuur en README van de formatieve opdracht volgens Guerilla Analytics: links) De 'directory tree' volgens de Guerilla Analytics regels. rechts) de inhoud van het readme bestand" width="100%" />
<p class="caption">(\#fig:opdracht 3a)Mapstructuur en README van de formatieve opdracht volgens Guerilla Analytics: links) De 'directory tree' volgens de Guerilla Analytics regels. rechts) de inhoud van het readme bestand</p>
</div>



## opdracht 3b
In deze opdracht heb ik de Guerrilla Analytics‑principes toegepast op mijn eigen portfolio‑repository. Ik heb de volledige projectstructuur opnieuw ingericht volgens de GA‑richtlijnen, waarbij ik een duidelijke scheiding heb aangebracht tussen data, code, documentatie, output en gegenereerde bestanden.

Daarnaast heb ik een nieuw README‑bestand opgesteld waarin ik de projectstructuur, gebruikte conventies en reproduceerbaarheid van het portfolio beschrijf.




``` r
library(png)
library(grid)
library(gridExtra)
library(here)

img1 <- rasterGrob(as.raster(readPNG(here::here("images", "dir_tree1.png"))))
img2 <- rasterGrob(as.raster(readPNG(here::here("images", "dir_tree2.png"))))
img3 <- rasterGrob(as.raster(readPNG(here::here("images", "dir_tree3.png"))))
img4 <- rasterGrob(as.raster(readPNG(here::here("images", "dir_tree4.png"))))
img5 <- rasterGrob(as.raster(readPNG(here::here("images", "read_me.png"))))

grid.arrange(img1, img2, img3,
             img4, img5,
             ncol = 3,
             top = textGrob("Portfolio volgens Guerrilla Analytics",
                            gp = gpar(fontsize = 10, font = 8)))
```

<div class="figure">
<img src="04_guerilla_analytics_files/figure-html/opdracht 3b-1.png" alt="Mapstructuur en README van portfolio map volgens Guerilla Analytics" width="100%" />
<p class="caption">(\#fig:opdracht 3b)Mapstructuur en README van portfolio map volgens Guerilla Analytics</p>
</div>
