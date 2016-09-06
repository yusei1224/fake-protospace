+db design
+===
+
+**table list**
+users
+prototypes
+comments
+images
+likes
+
+**users**
+*column*
+name :string
+email :text
+password :string
+profile_image :text
+
+**prototypes**
+concept :text
+catchcopy :text
+title :string
+user_id :integer
+
+**comments**
+content :text
+prototype_id :integer
+user_id :integer
+
+**likes**
+user_id :integer
+prototype_id :integer
+
+**images**
+image_url :text
+prototype_id :integer