<script lang="ts">
    import TopAppBar from '@smui/top-app-bar';
    import Row from '@smui/top-app-bar';
    import Section from '@smui/top-app-bar';
    import Title from '@smui/top-app-bar'
</script>
<div class="flexy">
    <div class="top-app-bar-container">
        <TopAppBar variant="static">
            <Row>
                <Section>
                    <Title>Saga</Title>
                </Section>
                <Section align="end" toolbar>
                    <h3>Lighttable</h3>
                    <h3>Gallery</h3>
                    <h3>Other</h3>
                </Section>
            </Row>
        </TopAppBar>
    </div>
</div>
<style>
    .top-app-bar-container {
        max-width: 480px;
        width: 100%;
        height: 320px;
        border: 1px solid;
        margin: 0 18px 18px 0;

        overflow: auto;
        display: inline-block;
    }
    .flexy {
        display: flex;
        flex-wrap: wrap;
    }
</style>