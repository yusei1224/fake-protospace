+db design
+===
+
+**table list**
+users
+prototypes
+comments
+prototype_images
+likes
+
+**users**
+*association*
+has_many :prototypes
+has_many :comments
+
+*column*
+name :string
+email :text
+password :string
+avatar :text
+member_of :text
+works :text
+profile :text
+
+**prototypes**
+*association*
+belongs_to :user
+has_many :likes
+has_many :prototype_images
+
+*column*
+concept :text
+catchcopy :text
+title :string
+user_id :integer
+
+**comments**
+*association*
+belongs_to :user
+
+*column*
+content :text
+prototype_id :integer
+user_id :integer
+
+**likes**
+*association*
+belongs_to :prototype
+
+*column*
+user_id :integer
+prototype_id :integer
+
+**prototype_images**
+*association*
+belongs_to :prototype
+*column*
+image :text
+status :{main_image: 0,sub_images: 1}
+prototype_id :integer

