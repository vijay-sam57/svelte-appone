<script>
  const student = {
    name: "",
    roll: "",
    bio: "",
    group: "",
    lang: [],
  };
  console.log(student);
</script>

<main>
  <form>
    <div>
      <label for="sname">Student's Name</label>
      <input type="text" id="sname" bind:value={student.name} />
    </div>
    <div>
      <label for="sroll">Student's Roll</label>
      <input type="number" id="sroll" bind:value={student.roll} />
    </div>
  </form>
  <div>
    <label for="sbio">Student's Bio</label>
    <textarea id="sbio" cols="30" rows="10" bind:value={student.bio} />
  </div>
  <div>
    <label for="sgroup">Student's Group</label>
    <select id="sgroup" bind:value={student.group}>
      <option value="">Select a group</option>
      <option value="Phy,Chem,Maths">PCM</option>
      <option value="Phy,Chem,Bio">PCB</option>
      <option value="Eco,Com,Acc">Eco</option>
    </select>
  </div>
  <div>
    <label for="plang">Programming Lang Known</label>
    <select id="plang" bind:value={student.lang} multiple>
      <option value="">Select known langs</option>
      <option value="C++">C++</option>
      <option value="Python">Python</option>
      <option value="Java">Java</option>
      <option value="Javascript">Javascript</option>
    </select>
  </div>
  <div>
    <h3>{student.name}</h3>
    <h3>{student.roll}</h3>
    <p>{student.bio}</p>
    <h4>{student.group}</h4>
    <h4>{student.lang}</h4>
  </div>
</main>

<style>
</style>
