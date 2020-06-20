Céation du blog avec RoR
    A) $ rails new nom_du_site_ou_app   (cree le dosssier et les fichier de base)
        1 => Base Model Vue Controller 
            - cree un dossier pour les pages de vue dans views (ex: pages)
            - cree pages d'accueil home (root 'dossier_vue#fichier_vue)
            - routes (dans routes.rb cree la route ex: get 'home', to:'pages#home') $ rake routes peut etre utile pour bien faire
            - controller (cree un fichier controller en minuscule ex: pages_controller)
                    *dans ce fichier creer une class du même nom en CamelCase ex :PagesController < ApplicationController avec def de chaque pages liées
            - views dans le dossier des vue crée avant, y crée les vues souhaitées (ex: home.html.erb)
            - tester le tout avec un $ rails s
                ** <%= le balise permet d'utiliser du code ruby dans le html %> 
                ** lien entres les differentes pages d'un memes dossier (tmp) 
                    * <%= link_to 'nom_qui_apparaitra_sur_le_site', root_path %>
            
        