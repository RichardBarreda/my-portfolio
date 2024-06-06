<template>
    <!-- Modal -->
<div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <h1 class="modal-title fs-5" id="exampleModalLabel">MESSAGE ME</h1>
                <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
            </div>
            <div class="modal-body">
                <form>
                    <div class="form-group">
                        <p class="form-label">Email Address:</p>
                        <input type="text" class="form-control">
                    </div>
                    <div class="form-group">
                        <p class="form-label">Subject:</p>
                        <input type="text" class="form-control">
                    </div>
                    <div class="form-group">
                        <p class="form-label">Message:</p>
                        <textarea type="text" class="form-control" rows="5"> </textarea>
                    </div>

                    <div class="form-btn">
                        <button type="button" class="btn btn-secondary btn-footer">CLEAR</button>
                        <button type="button" class="btn btn-success btn-footer">SUBMIT</button>
                    </div>
                </form>
            </div>
        </div>
    </div>
</div>
</template>
  



<script>
  export default {
    name: 'MessageMe',
    data() {
        return {

        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.form-btn {
    padding-top: 15px;
    display: flex;
    justify-content: flex-end;
}

.btn-secondary {
    margin-right: 10px;
}

.btn-footer {
    padding: 8px 30px;
}
</style>
  