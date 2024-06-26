# UCL_research_project

## To-Do List

<ul>
  <li>
    <input type="radio" id="task1" name="task-group">
    <label for="task1">Task 1</label> (Not Completed)
  </li>
  <li>
    <input type="radio" id="task2" name="task-group">
    <label for="task2">Task 2</label> (Not Completed)
  </li>
  </ul>



<script>
  const radios = document.querySelectorAll('input[type="radio"]');

  radios.forEach(radio => {
    radio.addEventListener('change', function() {
      const label = document.querySelector(`label[for="${this.id}"]`);
      if (this.checked) {
        label.classList.add('completed');
      } else {
        label.classList.remove('completed');
      }
    });
  });
</script>
