# Choses que j'ai apprises durant le projet Laravel X Vue

## Authentification
### AuthController
Ce fichier est un contrôleur Laravel, c’est-à-dire un fichier qui reçoit une requête HTTP (par exemple : /api/v1/register), fait des traitements, puis renvoie une réponse.

Il fait le lien entre le monde extérieur (ton front Vue) et le système Laravel (BDD, sessions, etc.).

**use Illuminate\Support\Facades\Hash;** : Cette ligne sert à utiliser le système de hachage de Laravel pour chiffrer les mots de passe.

Dans ce fichier AuthController.php, on va mettre toutes les méthodes liées à la création de compte, login, logout, etc.

**Comment ça fonctionne ?**

[ Front Vue ]
     ↓ POST /api/v1/register
[ Route Laravel ]
     ↓ appelle
[ AuthController@register ]
     ↓ crée
[ User dans la BDD ]
