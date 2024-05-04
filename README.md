Ce programme est une application de gestion de location de voitures écrite en langage C. Voici un rapport expliquant son fonctionnement et sa structure :Fonctions principales :
main() :
Cette fonction est le point d'entrée du programme.
Elle initialise les variables nécessaires, charge les données des voitures à partir du fichier CSV, puis affiche un menu interactif.
Selon le choix de l'utilisateur, elle appelle les différentes fonctions pour effectuer les opérations sur les voitures.Fonctions de gestion des voitures :
load_cars_from_file(Car *cars, int *num_cars) :
Charge les données des voitures à partir du fichier CSV dans le tableau cars.
Incrémente num_cars pour suivre le nombre de voitures chargées.
save_cars_to_file(Car *cars, int num_cars) :
Sauvegarde les données des voitures du tableau cars dans le fichier CSV.
Utilise le nombre actuel de voitures num_cars pour limiter le nombre de voitures à sauvegarder.
add_car(Car *cars, int *num_cars) :
Permet à l'utilisateur d'ajouter une nouvelle voiture en saisissant ses détails.
La nouvelle voiture est ajoutée à la fin du tableau cars et le nombre de voitures est incrémenté.
Les modifications sont ensuite sauvegardées dans le fichier CSV.
edit_car(Car *cars, int num_cars) :
Permet à l'utilisateur de modifier les détails d'une voiture en fonction de son ID.
Si la voiture est trouvée, l'utilisateur peut choisir de la modifier ou d'annuler l'opération.
Les modifications sont ensuite sauvegardées dans le fichier CSV.
delete_car(Car *cars, int *num_cars) :
Permet à l'utilisateur de supprimer une voiture en fonction de son ID.
Si la voiture est trouvée, l'utilisateur peut choisir de la supprimer ou d'annuler l'opération.
Les modifications sont ensuite sauvegardées dans le fichier CSV.
display_available_cars(Car *cars, int num_cars) :
Affiche la liste des voitures disponibles pour la location.
Parcourt le tableau cars et affiche les détails des voitures dont la disponibilité est "disponible".
Fonctions de recherche et de tri :
search_cars_by_brand(Car *cars, int num_cars) :
Permet à l'utilisateur de rechercher des voitures par marque.
Affiche les voitures dont la marque correspond à la recherche.
search_cars_by_availability(Car *cars, int num_cars) :
Permet à l'utilisateur de rechercher des voitures par disponibilité.
Affiche les voitures dont la disponibilité correspond à la recherche.
sort_cars_by_brand(Car *cars, int num_cars) :
Trie les voitures par marque dans l'ordre alphabétique.
Utilise l'algorithme de tri à bulles pour effectuer le tri.
sort_cars_by_price(Car *cars, int num_cars) :
Trie les voitures par prix de location par jour dans l'ordre croissant.
Utilise l'algorithme de tri à bulles pour effectuer le tri.
Fonctions utilitaires :
print_car_details(Car car) :
Affiche les détails d'une voiture spécifique passée en paramètre.
get_username(User *user) :
Demande à l'utilisateur de saisir son nom et le stocke dans la structure User.
clear_buffer() :
Vide le tampon d'entrée pour éviter les problèmes avec les prochaines entrées utilisateur.
Chaque fonction remplit un rôle spécifique dans la gestion des voitures et offre des fonctionnalités pour ajouter, modifier, supprimer, rechercher et trier les données des voitures, ce qui offre une expérience utilisateur complète dans cette application de gestion de location de voitures.
