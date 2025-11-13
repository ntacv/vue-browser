<script setup lang="ts">
import db from '@/data/firebase';
import {collection, doc, getDocs,setDoc} from "firebase/firestore"

const dbUser = collection(db, "user")


const querySnapshot = await getDocs(collection(db, "user"));
querySnapshot.forEach((doc) => {
  // doc.data() is never undefined for query doc snapshots
  console.log(doc.id, " => ", doc.data());
});

const data = querySnapshot.docs.map(doc => ({ id: doc.id, ...doc.data() }));

//const docId = data[0].id // && data.length > 0 ? data[0].id : null;

console.warn(data);

</script>
