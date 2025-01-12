# Lesson: Interaction Design

### First and Last Name: Konstantinos Lemonis
### University Registration Number: dpsd19065
### GitHub Personal Profile: https://github.com/Costas-Lemonis
### Augmented Reality Personal Repository: https://github.com/Costas-Lemonis/Augmented-Reality

# Introduction

# Summary


# 1st Deliverable
- (Cylinder)Αρχικά έκανα ένα καινούργιο `a-entity` για τον κύλινδρο με τον κώδικα από [εδώ](https://aframe.io/docs/1.3.0/components/geometry.html#cylinder) και άλλαξα το ύψος από 3 σε 2 και την ακτίνα από 2 σε 0.5

- (Sphere)Μετα έκανα ένα καινούργιο `a-entity` για την σφαίρα με τον κώδικα από [εδώ](https://aframe.io/docs/1.3.0/components/geometry.html#cylinder) και άλλαξα την ακτίνα από 2 σε 0.5

- (Snow)Έκανα προσθήκη τον **κώδικα** για το χιόνι από [εδώ](https://www.npmjs.com/package/aframe-particle-system-component) και μέσα στο a-entity έβαλα την εντολή `visible="false"` 
- (Speech Command)
  - Πρόσθεσα στον κώδικα το `a-entity id=annyang` από [εδώ](https://www.npmjs.com/package/aframe-speech-command-component)
  - Πρόσθεσα τον κώδικα για τα `speech-command_show` και `speech-command_hide` από [εδώ](https://www.npmjs.com/package/aframe-speech-command-component) στο a-entity με τον κώδικα από το χίονι, ώστε να εμφανίζεται και να εξαφανίζεται το χιόνι όταν λεμέ **start** και **stop** αντίστοιχα

# 2nd Deliverable
- (DPSD Marker)Αρχικά έκανα ένα καινούργιο `a-marker` για τον marker του DPSD19065 από [εδώ](https://www.oodlestechnologies.com/blogs/how-to-create-your-own-marker-for-ar-js/) μετά έφτιαξα τον marker στο **Affinity Designer** ώστε να γράφει πάνω το σωστό DPSD και δημιούργησα το αρχείο **.patt** από [εδώ](https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html) 
  - Μετά πρόσθεσα ένα `a-text` με τον **κώδικα** από [εδώ](https://levelup.gitconnected.com/simple-augmented-reality-ar-integration-with-a-frame-f625e9dc66b8) για να εμφανίζει το όνομα και το επίθετο και πείραξα το color και το position τους ![image](https://user-images.githubusercontent.com/100446886/168032754-19bbd3fe-7b13-4750-8e40-2b64cf18ca03.png)
  - Μετά πρόσθεσα ένα `a-image` με τον **κώδικα** από [εδώ](https://levelup.gitconnected.com/simple-augmented-reality-ar-integration-with-a-frame-f625e9dc66b8) για να εμφανίζει μια φωτογραφία της επιλογής μου και πείραξα το position ![image](https://user-images.githubusercontent.com/100446886/168034010-0028a7b6-0962-4d90-8389-cf3c874b760d.png)
- (Chemistry Project)Αρχικά οι markers έχουν `type=barcode` οπότε για να αναγνωρίζονται τα markers έπρεπε να προσθέσω τον binary code τους μέσα στο κεντρικό `a-scene` που βρήκα απο [εδώ](https://aframe.io/blog/arjs/) ![image](https://user-images.githubusercontent.com/100446886/168039775-f7419996-ef93-4b45-96de-d49c0ce3f363.png) οπότε ο κώδικα του html έγινε έτσι ![image](https://user-images.githubusercontent.com/100446886/168040674-dc1e8d65-d649-455e-809d-b985f233fe7e.png)
  - Μετά έκανα ένα `a-assets` για να ορίσω τα μοντέλο για το Hydrogen το οποίο έκανα στο **Blender** και το έκανα export σε .gltf [Video Texture](https://www.youtube.com/watch?v=r5YNJghc81U) ![image](https://user-images.githubusercontent.com/100446886/168044763-25343cc1-88c0-4fd1-9f50-7554506e2c5b.png)
  - Μετά έκανα ένα `a-assets` για να ορίσω τα μοντέλο για το Oxygen το οποίο έκανα στο **Blender** και το έκανα export σε .gltf [Video Texture](https://www.youtube.com/watch?v=r5YNJghc81U) ![image](https://user-images.githubusercontent.com/100446886/168046044-c8274f39-8baa-43d1-8cc4-60338e2ed8e1.png)
  - Μετά έκανα ένα `a-assets` για να ορίσω τα μοντέλο για το H2O το οποίο έκανα στο **Blender** και το έκανα export σε .gltf [Video Texture](https://www.youtube.com/watch?v=r5YNJghc81U) ![image](https://user-images.githubusercontent.com/100446886/168046173-950ac754-ac01-42e4-968c-d27f1c2a3fdc.png)

 - (Hydrogen Marker-H2O Marker)Μετά έκανα ένα καινούργιο `a-marker` για τον marker του Hydrogen με το κώδικα από [εδώ](https://aframe.io/blog/arjs/) και άλλαξα το **value** επίσης έφτιαξα τους marker στο **Affinity Designer** βάζοντας ένα απο τα barcode που βρήκα απο [εδώ](https://github.com/nicolocarpignoli/artoolkit-barcode-markers-collection)
   - Μετά πρόσθεσα ενα `a-image` μέσα στο marker έτσι ώστε να εμφανίζει την κάρτα του Hydrogen σαν φωτογραφία
   - Μετά πρόσθεσα ενα `a-entity` μέσα στο marker έτσι ώστε να να καλέσω το `a-assets` του Hydrogen και μετά πείραξα το position και το scale ώστε να φαίνεται καλύτερα
   - Μετά μέσα στον ίδιο Marker πρόσθεσα ενα `a-image` ώστε να να καλέσω το `a-assets` του H2O και έβαλα ενα `visible=false` ώστε να μην φαίνεται μαζί με την model του Hydrogen
   - Μετά μέσα στον ίδιο Marker πρόσθεσα ενα `a-entity` ώστε να εμφανίζει το μοντέλο του H2O και έβαλα ενα `visible=false` ώστε να μην φαίνεται μαζί με το Hydrogen

- (Oxygen Marker)Μετά έκανα ένα καινούργιο `a-marker` για τον marker του Oxygen με το κώδικα από [εδώ](https://aframe.io/blog/arjs/) και άλλαξα το **value**
   - Μετά πρόσθεσα ενα `a-image` μέσα στο marker έτσι ώστε να εμφανίζει την κάρτα του Oxygen σαν φωτογραφία
   - Μετά πρόσθεσα ενα `a-entity` μέσα στο marker έτσι ώστε να να καλέσω το `a-assets` του Oxygen και μετά πείραξα το position και το scale ώστε να φαίνεται καλύτερα και για το animation έβαλα την εντολή animation_rotate που βρήκα απο [εδώ](https://stemkoski.github.io/AR.js-examples/index.html)

- (Marker-Distance)Αρχικά έβαλα τον κώδικα για το `Script` από [εδώ](https://stackoverflow.com/questions/61239107/how-to-get-marker-position-x-y-ar-js)![image](https://user-images.githubusercontent.com/100446886/171505145-5a0dc592-8c36-4348-b539-a8cb6f3d3e29.png)
  και τον έφτιαξα έτσι ώστε να ταιρίαζει με τους markers ![image](https://user-images.githubusercontent.com/100446886/168085409-b152e9d7-db3f-4461-a633-b079635c9a56.png) Μετά έβαλα μια `if-else` έτσι ώστε αν ο **Marker-Distance < 2** τότε να εμφανίζει τον **Marker H2O** και να κρύβει τους **Markers** για το **Hydrogen**,**Oxygen** ενώ αν **Marker-Distance > 2** τότε να εμφανίζει τους **Markers** για το **Hydrogen**,**Oxygen** και να κρύβει τον **Marker H2O**

# 3rd Deliverable 
- (Place Of Interest)Αρχικά έκανα ένα `a-assets` για να ορίσω τα μοντέλο για την La Sagrada Família  το οποίο βρήκα από[εδώ](https://sketchfab.com/3d-models/sagrada-familia-front-facade-385d0c915b0b42e6829acae811f06fbe) ![image](https://user-images.githubusercontent.com/100446886/171505300-68ad7dae-b092-4428-9001-a47b42f3e95f.png)
 Μετά πρόσθεσα `position` και `scale` ώστε να φτιάξω το μέγεθος και την θέση του μοντέλου. Μετά έκανα ένα `a-text` για να προσθέσω το κείμενο για την περιγραφή του μοντέλου και πρόσθεσα `position` και `scale` ώστε να φτιάξω το μέγεθος και την θέση του κειμένου.
 Για το click event μετά από αρκετά παραδείγματα έκανα ένα mix από αυτούς τους κώδικες [κ.1](https://blog.davidvassallo.me/2019/09/26/augmented-reality-using-aframe-tips-tricks/)![image](https://user-images.githubusercontent.com/100446886/171506821-63327140-391a-4334-b1a4-4c9561dc6838.png)
 και [κ.2](https://glitch.com/~salty-partner-1)![image](https://user-images.githubusercontent.com/100446886/171507271-86dc14b3-2eb0-4309-baea-b0f5d9834c91.png)
 έπειτα πρόσθεσα ένα `class="click"` μέσα στο `a-entity` του μοντέλου και ένα `class="clickable"` μέσα στο `a-text` ώστε όταν κάνουμε click πάνω του να εμφανίζει το **text** Τέλος άλλαξα τα **Latitude** και **Longitude** με αυτά του Place Of Interest τα οποία βρήκα [εδώ](https://www.latlong.net/)
 
 - (Syros Place Of Interest)
Αρχικά άλλαξα τα **Latitude** και **Longitude** με αυτά του Syros Place Of Interest τα οποία βρήκα [εδώ](https://www.latlong.net/)
Μετά πρόσθεσα ένα `a-image` ώστε να εμφανίζει μια εικόνα από το μέρος που επέλεξα
Μετά πρόσθεσα ένα `a-text` ώστε να εμφανίζει ένα κείμενο από το μέρος που επέλεξα


# Conclusions


# Sources
- **Deliverable 1** | [Color Palettes](https://coolors.co/083d77-ebebd3-f4d35e-ee964b-f95738) | [Geometry](https://aframe.io/docs/1.3.0/components/geometry.html#cylinder#) | [Snow](https://www.npmjs.com/package/aframe-particle-system-component) | [Speech Command](https://www.npmjs.com/package/aframe-speech-command-component)
- **Deliverable 2** | [Marker Creator](https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html) | [3D Model Code](https://stemkoski.github.io/AR.js-examples/index.html) | [Animation](https://stemkoski.github.io/AR.js-examples/index.html) | [Barcode](https://github.com/nicolocarpignoli/artoolkit-barcode-markers-collection) | [Blender](https://www.blender.org/) | [Create Custom Marker](https://www.oodlestechnologies.com/blogs/how-to-create-your-own-marker-for-ar-js/) | [Blender Import Texture](https://www.youtube.com/watch?v=r5YNJghc81U) | [AR.js Examples](https://stemkoski.github.io/AR.js-examples/index.html)
- **Deliverable 3** | [Sagrada Familia 3D Model](https://sketchfab.com/3d-models/sagrada-familia-front-facade-385d0c915b0b42e6829acae811f06fbe) | [Touch Event EX.1](https://medium.com/swlh/how-to-handle-click-events-on-ar-js-f397ea5994d) | [Touch Event EX.2](https://medium.com/swlh/how-to-handle-click-events-on-ar-js-f397ea5994d)
| [Touch Event EX.3](https://glitch.com/~salty-partner-1) | [Touch Event EX.4](https://github.com/AR-js-org/AR.js/issues/216) | [Touch Event EX.5](https://stackoverflow.com/questions/63151052/click-event-on-a-entity-in-ar-js) | [Touch Event EX.6](https://stackoverflow.com/questions/63151052/click-event-on-a-entity-in-ar-js) | [Touch Event EX.7](https://medium.com/chialab-open-source/how-to-handle-click-events-on-ar-js-58fcacb77c4) | [Touch Event EX.8](https://www.w3.org/TR/touch-events/) | [Touch Event EX.9](https://ar-js-org.github.io/AR.js-Docs/ui-events/) | [Latitude and Longitude Finder](https://www.latlong.net/)
